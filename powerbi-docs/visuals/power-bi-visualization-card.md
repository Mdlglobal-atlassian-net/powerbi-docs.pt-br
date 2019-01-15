---
title: Visualizações de cartão (também conhecido como blocos de números grandes)
description: Criar uma Visualização de cartão no Power BI
author: mihart
manager: kvivek
ms.reviewer: ''
ms.service: powerbi
ms.subservice: powerbi-desktop
ms.topic: conceptual
ms.date: 09/26/2018
ms.author: mihart
LocalizationGroup: Visualizations
ms.openlocfilehash: 2bd35e5c2bc92ee660a9524754a3daef95e6e83d
ms.sourcegitcommit: c8c126c1b2ab4527a16a4fb8f5208e0f7fa5ff5a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2019
ms.locfileid: "54275791"
---
# <a name="card-visualizations"></a>Visualizações de cartão
Às vezes, um único número é a coisa mais importante que você deseja acompanhar no seu painel ou relatório do Power BI, como as vendas totais, a fatia de mercado ano após ano ou o total de oportunidades. Esse tipo de visualização é chamado de *Cartão*. Assim como em quase todas as visualizações nativas do Power BI, os cartões podem ser criados usando o editor de relatório ou P e R.

![visualização de cartão](media/power-bi-visualization-card/pbi_opptuntiescard.png)

## <a name="create-a-card-using-the-report-editor"></a>Criar um cartão usando o editor de relatório
Essas instruções usam o exemplo de análise de varejo. Para acompanhar, [baixe o exemplo](../sample-datasets.md) do serviço do Power BI (app.powerbi.com) ou do Power BI Desktop.   

1. Comece em uma página de relatório em branco e selecione **Armazenar** \> campo **Contagem de armazenamento aberto**. Caso esteja usando o serviço do Power BI, você precisará abrir o relatório no [Modo de Exibição de Edição](../service-interact-with-a-report-in-editing-view.md).

    O Power BI cria um gráfico de colunas com um número.

   ![](media/power-bi-visualization-card/pbi_rptnumbertilechart.png)
2. No painel de Visualizações, selecione o ícone de cartão.

   ![](media/power-bi-visualization-card/power-bi-templates.png)
6. Focalize sobre o cartão e selecione o ícone de pino ![](media/power-bi-visualization-card/pbi_pintile.png) para adicionar a visualização ao painel.

   ![](media/power-bi-visualization-card/power-bi-pin-icon.png)
7. Fixe o bloco em um painel existente ou em um novo painel.

   * Painel existente: selecione o nome do painel no menu suspenso.
   * Novo painel: digite o nome do novo painel.
8. Selecione **Fixar**.

   Uma mensagem de Êxito (perto do canto superior direito) informa que a visualização foi adicionada, como um bloco, ao painel.

   ![](media/power-bi-visualization-card/power-bi-success2.png)
9. Selecione **Ir para o dashboard**. Nele, você pode [editar e mover](../service-dashboard-edit-tile.md) a visualização fixada.


## <a name="create-a-card-from-the-qa-question-box"></a>Criar um cartão a partir de uma caixa de perguntas de P e R
A caixa pergunta de P e R é a maneira mais fácil de fazer um Cartão. A caixa de perguntas P e R está disponível no serviço do Power BI de um dashboard ou relatório e na exibição de relatório da Área de Trabalho. As etapas abaixo descrevem como criar um Cartão a partir de um painel do serviço do Power BI. Se você deseja criar um cartão usando um P e R no Power BI Desktop, [siga estas instruções](https://powerbi.microsoft.com/en-us/blog/power-bi-desktop-december-feature-summary/#QandA) para a versão prévia do P e R para relatórios do Desktop.

1. Crie um [dashboard](../service-dashboards.md) e [obtenha dados](../service-get-data.md). Este exemplo usa a [amostra Análise de Oportunidade](../sample-opportunity-analysis.md).

1. Na parte superior do painel, comece a digitar o que você deseja saber sobre os dados na caixa de pergunta. 

   ![](media/power-bi-visualization-card/power-bi-q-and-a-box.png)

> [!TIP]
> Em um relatório de serviço do Power BI, na **Exibição de edição**, selecione Fazer uma pergunta na barra de menus superior. Em um relatório do Power BI Desktop, encontre algum espaço aberto e clique duas vezes para abrir uma caixa de pergunta.

3. Por exemplo, digite “número de oportunidades” na caixa de pergunta.

   ![](media/power-bi-visualization-card/power-bi-q-and-a.png)

   A caixa da pergunta o ajuda dando sugestões e reformulações e, por fim, exibe o número total.  
4. Selecione o ícone de pino ![](media/power-bi-visualization-card/pbi_pintile.png) no canto superior direito para adicionar o cartão ao painel.

   ![](media/power-bi-visualization-card/power-bi-pin.png)
5. Fixe o cartão, com um bloco, em um painel existente ou novo.

   * Painel existente: selecione o nome do painel no menu suspenso. Suas opções serão limitadas apenas aos dashboards no workspace atual.
   * Novo dashboard: digite o nome do novo dashboard e ele será adicionado ao seu workspace atual.
6. Selecione **Fixar**.

   Uma Mensagem de êxito (perto do canto superior direito) informa que a visualização foi adicionada, como um bloco, ao painel.  

   ![](media/power-bi-visualization-card/power-bi-success2.png)
7. Selecione **Ir para o dashboard** para ver o novo bloco. Nele, é possível [renomear, redimensionar, adicionar um hiperlink, reposicionar o bloco e muito mais](../service-dashboard-edit-tile.md) no dashboard.

   ![](media/power-bi-visualization-card/power-bi-pinned.png)

## <a name="considerations-and-troubleshooting"></a>Considerações e solução de problemas
- Se uma caixa de perguntas não for exibida, entre em contato com o administrador do sistema ou de locatário.    
- Se você estiver usando a área de trabalho e, ao clicar duas vezes em um espaço vazio de um relatório, o P e R não abrir, você precisará ativá-lo.  Selecione **Arquivo > Opções e Configurações > Opções > Recursos de versão prévia > P e R** e reinicie o Desktop.

## <a name="format-a-card"></a>Formatar um cartão
Você tem várias opções para alterar rótulos, texto, cor e muito mais. A melhor maneira de aprender é criar um cartão e, em seguida, explorar o painel de formatação. Aqui estão algumas das opções de formatação disponíveis. 

1. Comece selecionando o ícone de rolo de tinta para abrir o painel Formatação. 

    ![cartão com rolo de tinta descrito](media/power-bi-visualization-card/power-bi-format-card.png)
2. Expanda **Rótulo de dados** e altere a cor, o tamanho e a família de fontes. Se você tivesse milhares de repositórios, poderia usar **Exibir unidades** para mostrar o número de repositórios por milhares e controlar as casas decimais também. Por exemplo, 125,8K em vez de 125.832,00.

3.  Expanda **Rótulo de categoria** e altere a cor e o tamanho.

    ![cor azul-escura selecionada](media/power-bi-visualization-card/power-bi-card-format.png)

4. Expanda **Plano de fundo** e mova o controle deslizante para ligado.  Agora você pode alterar a cor da tela de fundo e a transparência.

    ![controle deslizante definido como LIGADO](media/power-bi-visualization-card/power-bi-format-color.png)

5. Continue para explorar as opções de formatação até que seu cartão esteja exatamente como você deseja. 

    ![Cartão depois de toda a formatação estar concluída](media/power-bi-visualization-card/power-bi-formatted.png)

## <a name="next-steps"></a>Próximas etapas
[Gráficos de combinação no Power BI](power-bi-visualization-combo-chart.md)

[Tipos de visualização no Power BI](power-bi-visualization-types-for-reports-and-q-and-a.md)
