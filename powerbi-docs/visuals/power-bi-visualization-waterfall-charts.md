---
title: Gráficos de cascata no Power BI
description: Gráficos de cascata no Power BI
author: mihart
manager: kvivek
ms.reviewer: ''
featuredvideoid: maTzOJSRB3g
ms.service: powerbi
ms.subservice: powerbi-desktop
ms.topic: conceptual
ms.date: 09/27/2018
ms.author: mihart
LocalizationGroup: Visualizations
ms.openlocfilehash: 3835bedc1b4ab2df87abf4704ef338ff7f4abc5d
ms.sourcegitcommit: 60dad5aa0d85db790553e537bf8ac34ee3289ba3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/29/2019
ms.locfileid: "61392919"
---
# <a name="waterfall-charts-in-power-bi"></a>Gráficos de cascata no Power BI
O gráfico de cascata mostram uma duração total conforme os valores são adicionados ou subtraídos. É útil para entender como um valor inicial (por exemplo, a receita líquida) é afetado por uma série de alterações positivas e negativas.

As colunas são codificadas para que você possa rapidamente aumentar e diminuir. Com frequência, as colunas de valor inicial e final [iniciam-se no eixo horizontal](https://support.office.com/article/Create-a-waterfall-chart-in-Office-2016-for-Windows-8de1ece4-ff21-4d37-acd7-546f5527f185#BKMK_Float "iniciam-se no eixo horizontal"), enquanto os valores intermediários são colunas flutuantes. Devido a essa "aparência", os gráficos de cascata também são chamados de gráficos de ponte.

<iframe width="560" height="315" src="https://www.youtube.com/embed/qKRZPBnaUXM" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

## <a name="when-to-use-a-waterfall-chart"></a>Ao usar um gráfico de cascata
Os gráficos de cascata são uma ótima opção:

* quando houver alterações de medida em uma série de tempo ou categorias diferentes
* para auditar as principais alterações que contribuem para o valor total
* para traçar o lucro anual da empresa, mostrando várias fontes de receita e chegar ao lucro total (ou perda).
* para ilustrar o início e final do número de funcionários de sua empresa em um ano
* para visualizar a quantidade de dinheiro, faça e gaste todo mês e o saldo parcial para sua conta. 

## <a name="create-a-waterfall-chart"></a>Criar um gráfico de cascata
Criaremos um gráfico de cascata que exibe a variação de vendas (vendas estimadas versus vendas reais) por mês. Para acompanhar, entre no Power BI e selecione **Obter Dados \> Amostras \> Amostra de Análise de Varejo**. 

1. Selecione a guia **Conjuntos de dados** e role até o novo conjunto de dados "Exemplo de Análise de Varejo".  Selecione o ícone **Criar relatório** para abrir o conjunto de dados no modo de exibição de edição de relatório. 
   
    ![Guia Conjuntos de Dados realçada](media/power-bi-visualization-waterfall-charts/power-bi-waterfall-report.png)
2. No painel **Campos**, selecione **Vendas \> Variação do Total de Vendas**. 
3. Converter o gráfico para uma **Cascata**. Se a **Variação Total de Vendas** não está na área do **eixo Y** , arraste-o para lá.
   
    ![Modelos de visualização](media/power-bi-visualization-waterfall-charts/convertwaterfall.png)
4. Selecione **Hora** \> **FiscalMonth** para adicioná-la à seção **Categoria**. 
   
    ![cascata](media/power-bi-visualization-waterfall-charts/power-bi-waterfall.png)
5. Classifique o gráfico de cascata em ordem cronológica. No canto direito do gráfico, selecione as reticências (...) e **FiscalMonth**.
   
    ![escolha classificar por > FiscalMonth](media/power-bi-visualization-waterfall-charts/power-bi-sort-by.png)
   
    ![resultado da nova classificação ascendente](media/power-bi-visualization-waterfall-charts/power-bi-waterfall-sorted.png)
6. Aprofunde-se um pouco mais para ver o que está contribuindo mais para as alterações a cada mês. Arraste **Repositório** > **Região** para o bucket **Divisão**.
   
    ![Mostra Repositório no bucket de Divisão](media/power-bi-visualization-waterfall-charts/power-bi-waterfall-breakdown.png)
7. Por padrão, o Power BI adiciona os cinco principais colaboradores a aumentos ou diminuições por mês. Mas queremos apenas os dois colaboradores principais.  No painel de formatação, selecione **Divisão** e defina **Máximo** como 2.
   
    ![Formatação > Divisão](media/power-bi-visualization-waterfall-charts/power-bi-waterfall-breakdown-maximum.png)
   
    Uma rápida análise revela que as regiões de Ohio e Pensilvânia são os maiores colaboradores para a movimentação, negativa e positiva, em nosso gráfico de cascata. 
   
    ![gráfico de cascata](media/power-bi-visualization-waterfall-charts/power-bi-waterfall-axis.png)
8. Essa é uma descoberta interessante. Ohio e Pensilvânia têm um impacto significativo por as vendas nessas duas regiões serem muito maiores do que nas outras?  Podemos verificar isso. Crie um mapa que examina o valor de vendas deste ano e as vendas do último ano por território.  
   
    ![close-up do mapa em PA e Ohio](media/power-bi-visualization-waterfall-charts/power-bi-map.png)
   
    Nosso mapa corrobora nossa teoria.  Ele mostra que essas duas regiões tiveram o valor mais alto de vendas no ano passado (tamanho da bolha) e neste ano (sombreamento da bolha).

## <a name="highlighting-and-cross-filtering"></a>Realce e filtragem cruzada
Para obter informações sobre como usar o painel Filtros, veja [Adicionar um filtro a um relatório](../power-bi-report-add-filter.md).

Realçar uma coluna em um gráfico de cascata faz a filtragem cruzada dos filtros com outras visualizações na página do relatório e vice-versa. No entanto, a coluna Total não dispara o realce ou responda a filtragem cruzada.

## <a name="next-steps"></a>Próximas etapas

[Interações visuais](../service-reports-visual-interactions.md)

[Tipos de visualização no Power BI](power-bi-visualization-types-for-reports-and-q-and-a.md)