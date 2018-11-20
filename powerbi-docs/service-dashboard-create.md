---
title: Criar um dashboard do Power BI de um relatório
description: Criar um dashboard do Power BI de um relatório
author: maggiesMSFT
manager: kfile
ms.reviewer: ''
featuredvideoid: ''
ms.service: powerbi
ms.component: powerbi-service
ms.topic: conceptual
ms.date: 10/02/2018
ms.author: maggies
ms.openlocfilehash: 28a282ff6a35061422995c46fbbcd34c21b533a7
ms.sourcegitcommit: 1e4fee6d1f4b7803ea285eb879c8d5a4f7ea8b85
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2018
ms.locfileid: "51717414"
---
# <a name="create-a-power-bi-dashboard-from-a-report"></a>Criar um dashboard do Power BI de um relatório
Você já leu [Dashboards no Power BI](service-dashboards.md) e agora deseja criar o seu próprio. Há várias maneiras diferentes de criar um dashboard de controle – de um relatório, desde o início, de um conjunto de dados, duplicando um dashboard existente e muito mais.  

Pode parecer complicado quando você está começando, então vamos começar criando um painel rápido e fácil fixando visualizações de um relatório que já esteja criado. Depois de concluir este guia de início rápido, você terá um bom entendimento da relação entre painéis e relatórios, de como abrir o modo de exibição de edição no editor de relatórios, como fixar blocos e navegar entre um painel e um relatório. Em seguida, use os links no sumário à esquerda ou **Próximas etapas** na parte inferior para passar para os tópicos mais avançados.

## <a name="who-can-create-a-dashboard"></a>Quem pode criar um painel?
Criar um painel é um recurso do **criador** e requer permissões de edição para o relatório. As permissões de edição estão disponíveis para os criadores do relatório e os colegas aos quais o criador concede acesso. Por exemplo, se David criar um relatório no workspaceABC e, em seguida, o adicionar como membro desse workspace, você e David terão permissão de edição. Por outro lado, se um relatório tiver sido compartilhado com você diretamente ou como parte de um [aplicativo do Power BI](service-create-distribute-apps.md) (você está **consumindo** o relatório), não será possível fixar blocos em um painel.

> **OBSERVAÇÃO**: os dashboards são um recurso do serviço do Power BI, não do Power BI Desktop. Os dashboards não podem ser criados em dispositivos móveis Power BI, mas podem ser [exibidos e compartilhados](consumer/mobile/mobile-apps-view-dashboard.md).
>
> 

![dashboard](media/service-dashboard-create/power-bi-completed-dashboard-small.png)

## <a name="video-create-a-dashboard-by-pinning-visuals-and-images-from-a-report"></a>Vídeo: criar um dashboard fixando visuais e imagens de um relatório
Veja a Amanda criar um novo dashboard fixando visualizações de um relatório. Em seguida, siga as etapas abaixo do vídeo para tentar você mesmo, usando o exemplo de análise de compras.

<iframe width="560" height="315" src="https://www.youtube.com/embed/lJKgWnvl6bQ" frameborder="0" allowfullscreen></iframe>

### <a name="prerequisites"></a>Pré-requisitos
Para acompanhar, você precisará baixar a pasta de trabalho do Excel de exemplo "Análise de compras" e abri-la no serviço Power BI (app.powerbi.com).

## <a name="import-a-dataset-with-a-report"></a>Importar um conjunto de dados com um relatório
Vamos importar um dos conjuntos de dados de exemplo do Power BI e usá-lo para criar nosso novo dashboard. O exemplo que usaremos é uma pasta de trabalho do Excel com duas planilhas do PowerView. Quando o Power BI importar a pasta de trabalho, ele adicionará um conjunto de dados e também um relatório ao seu workspace.  O relatório é criado automaticamente das planilhas do PowerView.

1. [Clique neste link](http://go.microsoft.com/fwlink/?LinkId=529784) para baixar e salvar o arquivo de Excel de exemplo de análise de compras. É recomendável salvá-lo em seu OneDrive for Business.
2. Abra o serviço do Power BI no seu navegador (app.powerbi.com).
3. Selecione **Meu Workspace**.
4. No painel de navegação esquerdo, selecione **Obter Dados**.

    ![painel de navegação esquerdo](media/service-dashboard-create/power-bi-get-data3.png)
5. Selecione **Arquivos**.

   ![Obter arquivos](media/service-dashboard-create/power-bi-select-files.png)
6. Navegue até o local em que você salvou o arquivo do Excel de exemplo de análise de compras. Selecione-o e escolha **Conectar**.

   ![conectar-se a arquivos](media/service-dashboard-create/power-bi-connectnew.png)
7. Para este exercício, selecione **Importar**.

    ![Janela OneDrive para Empresas](media/service-dashboard-create/power-bi-import.png)
8. Quando a mensagem de êxito for exibida, selecione o **x** para fechá-la.

   ![mensagem de êxito](media/service-dashboard-create/power-bi-view-datasetnew.png)

### <a name="open-the-report-and-pin-some-tiles-to-a-dashboard"></a>Abra o relatório e fixe alguns blocos em um dashboard
1. Permanecendo no mesmo workspace, selecione a guia **Relatórios**. O relatório importado recentemente é exibido com um asterisco amarelo. Selecione o nome do relatório para abri-lo.

    ![guia relatórios](media/service-dashboard-create/power-bi-reports.png)
2. O relatório é aberto no modo de exibição de Leitura. Observe que ele tem duas guias na parte inferior: Análise de desconto e Visão geral de gastos. Cada guia representa uma página do relatório.
    Selecione **Editar relatório** para abrir o relatório no modo de exibição de Edição.

    ![relatório em modo de exibição de Leitura](media/service-dashboard-create/power-bi-reading-view.png)
3. Passe o mouse sobre uma visualização para revelar as opções disponíveis. Para adicionar a visualização a um dashboard, selecione o ícone ![](media/service-dashboard-create/power-bi-pin-icon.png) de fixação.

    ![passar o mouse sobre o bloco](media/service-dashboard-create/power-bi-hover.png)
4. Como estamos criando um novo dashboard, selecione a opção **Novo painel** e dê um nome.

   ![Caixa de diálogo Fixar no dashboard](media/service-dashboard-create/power-bi-pin-tile.png)
5. Ao selecionar **Fixar**, o Power BI criará o novo dashboard no workspace atual. Quando a mensagem **Fixado ao painel** for exibida, selecione **Ir para o dashboard**. Se for solicitado salvar o relatório, escolha **Salvar**.

     ![mensagem de êxito](media/service-dashboard-create/power-bi-pin-success.png)
6. O Power BI abre o novo painel e há um bloco – a visualização que você acabou de fixar.

   ![dashboard com um bloco](media/service-dashboard-create/power-bi-pinned.png)
7. Para retornar ao relatório, selecione o bloco. Fixe mais alguns blocos ao novo dashboard. Desta vez, quando a janela **Fixar no Painel** for exibida, selecione **Painel Existente**.  

   ![Caixa de diálogo Fixar no dashboard](media/service-dashboard-create/power-bi-existing-dashboard.png)

## <a name="pin-an-entire-report-page-to-the-dashboard"></a>Fixar uma página inteira do relatório no painel
Em vez de fixar um visual de cada vez, você pode [fixar uma página inteira do relatório como um *bloco dinâmico*](service-dashboard-pin-live-tile-from-report.md). Vamos fazer isso.

1. No editor de relatórios, selecione a guia **Visão geral de gastos** para abrir a página 2 do relatório.

   ![guia relatório](media/service-dashboard-create/power-bi-page-tab.png)

2. Você quer todos esses elementos visuais no painel.  No canto superior direito da barra de menus, selecione **Fixar página dinâmica**. Em um painel, os blocos de página dinâmica são atualizados cada vez que a página é atualizada.

   ![canto superior direito do editor de relatório](media/service-dashboard-create/power-bi-pin-live.png)

3. Quando a janela **Fixar no Painel** for exibida, selecione **Painel Existente**.

   ![Caixa de diálogo Fixar no dashboard](media/service-dashboard-create/power-bi-pin-live2.png)

4. Quando a mensagem de Êxito for exibida, selecione **Ir para o painel**. Lá você verá os blocos fixados a partir do relatório. No exemplo a seguir, fixamos 2 blocos da página 1 do relatório e um bloco dinâmico que é a página 2 do relatório.

   ![dashboard](media/service-dashboard-create/power-bi-dashboard.png)

Parabéns! Você criou seu primeiro dashboard! Agora que você tem um dashboard, há muito mais que você pode fazer com ele.  Tente uma das **próximas etapas** sugeridas abaixo ou comece a testar e explorar por conta própria.   

## <a name="next-steps"></a>Próximas etapas
* [Redimensionar e mover blocos](service-dashboard-edit-tile.md)
* [Tudo sobre blocos de dashboard](service-dashboard-tiles.md)
* [Compartilhar seu dashboard criando um aplicativo](service-create-workspaces.md)
* [Power BI – conceitos básicos](service-basic-concepts.md)
* [Dicas para projetar um ótimo dashboard](service-dashboards-design-tips.md)

Mais perguntas? [Experimente a Comunidade do Power BI](http://community.powerbi.com/)
