---
title: Gráficos de funil
description: Gráficos de funil no Power BI
author: mihart
manager: kvivek
ms.reviewer: ''
featuredvideoid: maTzOJSRB3g
ms.service: powerbi
ms.subservice: powerbi-desktop
ms.topic: conceptual
ms.date: 06/12/2019
ms.author: mihart
LocalizationGroup: Visualizations
ms.openlocfilehash: b12b2035d7686667535dfdddba42b4b8ca014d96
ms.sourcegitcommit: 4ae1257c5d7b33aa2fafd91caf8b353a985c6771
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2019
ms.locfileid: "67161118"
---
# <a name="funnel-charts"></a>Gráficos de funil
Um gráfico de funil ajuda você a visualizar um processo linear com estágios conectados sequenciais. Por exemplo, um funil de vendas que acompanha clientes pelos estágios: Oportunidade \> Oportunidade qualificada \> Cliente potencial \> Contrato \> Fechamento.  Em um relance, a forma do funil transmite a integridade do processo que você está controlando.

Cada estágio de funil representa um percentual do total. Portanto, na maioria dos casos, um gráfico de funil tem a forma de um funil – com o primeiro estágio sendo o maior, e cada estágio subsequente, menor do que seu antecessor.  Um funil em forma de pera também é útil - ele pode identificar um problema no processo.  Mas, em geral, o primeiro estágio, o estágio de "entrada", é o maior.

![exemplo de funil azul](media/power-bi-visualization-funnel-charts/funnelplain.png)

## <a name="when-to-use-a-funnel-chart"></a>Quando usar um gráfico de funil
Os gráficos de funil são uma ótima opção:

* Quando os dados são sequenciais e se movimentam em pelo menos 4 estágios.
* Quando o número de "itens" no primeiro for maior que o número no estágio final.
* calcular o potencial (receita de vendas/negociações/etc.) por estágios.
* calcular e controlar as taxas de conversão e retenção.
* revelar afunilamentos em um processo linear.
* controlar o fluxo de trabalho do carrinho de compras.
* rastrear o progresso e o sucesso das campanhas de propaganda/marketing.

## <a name="working-with-funnel-charts"></a>Como trabalhar com gráficos de funil
Gráficos de funil:

* Podem ser fixado por meio dos relatórios e de perguntas e respostas.
* Podem ser classificados.
* Vários suportes.
* Podem ser realçados e cruzados por outras visualizações na mesma página de relatório.
* Podem ser usados para destacar e cruzar outras visualizações na mesma página de relatório.

## <a name="create-a-basic-funnel-chart"></a>Criar um gráfico de funil básico
Assista a este vídeo para ver Will criar um gráfico de Funil usando a amostra de Vendas e Marketing.

<iframe width="560" height="315" src="https://www.youtube.com/embed/qKRZPBnaUXM" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>


Agora crie seu próprio gráfico de funil que mostra o número de oportunidades que temos em cada um de nossos estágios de vendas.

Essas instruções usam o Exemplo de Análise de Oportunidade. Para acompanhar, [baixe o exemplo](../sample-datasets.md) do serviço do Power BI (app.powerbi.com) ou do Power BI Desktop.   

1. Comece em uma página de relatório em branco e selecione o campo **SalesStage** \> **Sales Stage**. Caso esteja usando o serviço do Power BI, certifique-se de abrir o relatório no [Modo de Exibição de Edição](../service-interact-with-a-report-in-editing-view.md).
   
    ![selecionar estágio de vendas](media/power-bi-visualization-funnel-charts/funnelselectfield_new.png)
2. [Converta o gráfico](power-bi-report-change-visualization-type.md) em um funil. Observe que **Estágio de Vendas** está no contêiner **Grupo** . 
3. No painel **Campos**, selecione **Fato** \> **Contagem de Oportunidades**.
   
    ![criar o gráfico de funil](media/power-bi-visualization-funnel-charts/power-bi-funnel-2.png)
4. Passar o mouse sobre uma barra exibe uma variedade de informações.
   
   * O nome do estágio
   * Número de oportunidades no momento deste estágio
   * Taxa de conversão geral (% do cliente potencial) 
   * Passo a passo (também conhecido como taxa de eliminação) que é % do estágio anterior (nesse caso, Estágio de Proposta/Estágio de Solução)
     
     ![detalhes da barra Proposta](media/power-bi-visualization-funnel-charts/funnelhover_new.png)
5. [Adicionar o Funil como um bloco do dashboard](../service-dashboard-tiles.md). 
6. [Salve o relatório](../service-report-save.md).

## <a name="highlighting-and-cross-filtering"></a>Realce e filtragem cruzada
Para obter informações sobre como usar o painel Filtros, veja [Adicionar um filtro a um relatório](../power-bi-report-add-filter.md).

Realçar uma barra em um funil faz a filtragem cruzada das outras visualizações na página do relatório e vice-versa. Para acompanhar, adicione mais alguns elementos visuais à página do relatório que contém o gráfico de funil.

1. No funil, selecione a barra **Proposta**. Isso destaca de forma cruzada as outras visualizações na página. Use CTRL para fazer uma seleção múltipla.
   
   ![breve vídeo mostrando interações de visuais](media/power-bi-visualization-funnel-charts/funnelchartnoowl.gif)
2. Para definir as preferências de como os visuais são realçados e filtrados de forma cruzada entre si, veja [Interações de visuais no Power BI](../service-reports-visual-interactions.md)

## <a name="create-a-funnel-chart-using-qa"></a>Criar um gráfico de funil usando P e R
Abra o painel de Exemplo de Análise de Oportunidade ou qualquer outro painel que tenha pelo menos uma visualização fixada do conjunto de dados de Exemplo de Análise de Oportunidade.  Quando você digitar uma pergunta em P e R, o Power BI procura por respostas em todos os conjuntos de dados associados (blocos fixados) ao o painel selecionado. Para obter mais informações, veja [Power BI – Conceitos básicos](../service-basic-concepts.md).

1. No painel de Exemplo de Análise de Oportunidade, comece a digitar sua pergunta na caixa de perguntas P e R.
   
   ![caixa de pergunta e funil](media/power-bi-visualization-funnel-charts/power-bi-qna.png)
   
2. Certifique-se de adicionar "como funil" para o que Power BI saiba qual tipo de visualização você prefere.

## <a name="next-steps"></a>Próximas etapas

[Medidores no Power BI](power-bi-visualization-radial-gauge-charts.md)

[Tipos de visualização no Power BI](power-bi-visualization-types-for-reports-and-q-and-a.md)
