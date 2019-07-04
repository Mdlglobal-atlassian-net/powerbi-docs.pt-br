---
title: A nova experiência de filtro em relatórios do Power BI (versão prévia)
description: Os filtros no Power BI estão recebendo novas funcionalidades e um novo design.
author: maggiesMSFT
manager: kfile
ms.reviewer: ''
ms.service: powerbi
ms.subservice: powerbi-service
ms.topic: conceptual
ms.date: 06/25/2019
ms.author: maggies
LocalizationGroup: Reports
ms.openlocfilehash: 6a95ddd8f13be2407736c126b087723ceb5d9f31
ms.sourcegitcommit: 58c649ec5fd2447a0f9ca4c4d45a0e9fff2f1b6a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "67409158"
---
# <a name="the-new-filter-experience-in-power-bi-reports-preview"></a>A nova experiência de filtro em relatórios do Power BI (versão prévia)

Os filtros no Power BI têm novas funcionalidades e um novo design. Ao escolher a nova experiência de filtro, será possível formatar o painel Filtros para se parecer com o restante do relatório. Você poderá bloquear e ocultar até mesmo filtros. Ao criar seu relatório, você não verá mais o painel Filtros antigo no painel Visualizações. É possível editar e formatar todos os filtros no painel Filtros. 

![Nova experiência de filtro](media/power-bi-report-filter-preview/power-bi-filter-reading.png)

> [!NOTE]
> A nova experiência de filtro está em versão prévia. Os novos builds podem substituir a formatação já definida.

Veja a seguir o que você pode fazer no novo e exclusivo painel Filtros enquanto cria um relatório:

- Adicionar e remover campos para filtrar. 
- Alterar o estado do filtro.
- Formatar e personalizar o painel Filtros para que ele se integre ao relatório.
- Definir se o painel Filtros fica aberto ou recolhido por padrão quando um consumidor abre o relatório.
- Ocultar todo o painel Filtros ou filtros específicos que você não deseja exibir aos consumidores do relatório.
- Controlar e até mesmo marcar o estado de visibilidade aberto e recolhido do novo painel Filtros.
- Bloquear filtros os quais você não deseja que os consumidores editem.

Com a nova experiência de filtro, os consumidores do relatório podem também passar o mouse sobre qualquer visual para ver uma lista somente leitura de todos os filtros ou segmentações que afetam esse visual.

![Lista de filtros para um visual](media/power-bi-report-filter-preview/power-bi-filter-visual.png)

## <a name="turn-on-the-new-filter-experience"></a>Ativar a nova experiência de filtro 

Habilite a nova experiência no Power BI Desktop. Depois, você pode modificar os filtros nele ou no serviço do Power BI (https://app.powerbi.com). Como essa nova experiência de filtro está em versão prévia, primeiro você precisa habilitá-la no Power BI Desktop. Se você iniciar criando um relatório no serviço do Power BI, ele não poderá ter os novos filtros.

### <a name="turn-on-new-filters-for-all-new-reports"></a>Ativar novos filtros para todos os relatórios novos

1. No Power BI Desktop, selecione **Arquivo** > **Opções e Configurações** > **Opções** > **Recursos de Visualização** e marque a caixa de seleção **Nova experiência de filtro**. 
2. Reinicie o Power BI Desktop para ver a nova experiência de filtro em todos os relatórios novos.

Depois de reiniciar o Power BI Desktop, ela fica habilitada por padrão para todos os novos relatórios criados.  

### <a name="turn-on-new-filters-for-an-existing-report"></a>Ativar novos filtros para um relatório existente

Você também pode habilitar os novos filtros para relatórios existentes.

1. No Power BI Desktop, em um relatório existente, selecione **Arquivo** > **Opções e Configurações** > **Opções**
2. Na barra de navegação à esquerda, em **Arquivo atual**, selecione **Configurações de relatório**.
3. Em **Experiência de filtragem**, selecione **Habilitar o painel de filtros atualizado e mostrar filtros no cabeçalho do visual para este relatório**.

## <a name="view-filters-for-a-visual-in-reading-mode"></a>Ver filtros para um visual no modo Leitura

No Modo de Leitura, você pode passar o mouse sobre o ícone de filtro em um visual para ver um pop-up com todos os filtros, segmentações, etc., que afetam esse visual. A formatação de pop-up é igual à formatação do painel Filtros. 

![Filtros que afetam um visual](media/power-bi-report-filter-preview/power-bi-filter-per-visual.png)

Estes são os tipos de filtros mostrados por essa exibição: 
- Filtros básicos
- Segmentações
- Realce cruzado 
- Filtragem cruzada
- Filtros avançados
- Primeiros N filtros
- Filtros de Data Relativa
- Sincronizar segmentadores
- Incluir/Excluir filtros
- Filtros passados por uma URL

## <a name="build-the-new-filters-pane"></a>Criar o novo painel Filtros

Depois de habilitar o novo painel Filtros, você pode vê-lo à direita da página do relatório, formatado por padrão com base nas configurações de relatório atuais. Use o novo painel Filtros para configurar os filtros incluídos e atualizar os filtros existentes no novo painel. O novo painel Filtros mostra o que os consumidores do relatório verão quando você publicar o relatório. 

1. Por padrão, os leitores do relatório podem ver o painel Filtros. Se não quiser que eles vejam, selecione o ícone de olho ao lado de **Filtros**.

    ![Ícone de olho de filtro do Power BI](media/power-bi-report-filter-preview/power-bi-filter-eye.png)

2. Para começar a criar o novo painel Filtros, arraste os campos de interesse para o novo painel Filtros, como filtros de nível visual, de página ou de relatório.

Quando você adiciona um visual a uma tela de relatório, o Power BI adiciona automaticamente um filtro ao painel Filtros para cada campo no visual. 

## <a name="lock-or-hide-filters"></a>Bloquear ou ocultar filtros

Você pode bloquear ou ocultar os cartões de filtro individuais. Se você bloquear um filtro, os consumidores do relatório poderão vê-lo, mas não alterá-lo. Se você ocultá-lo, eles não poderão nem vê-lo. Ocultar os cartões de filtro é útil se você precisar ocultar filtros de limpeza de dados que excluem valores nulos ou inesperados. 

- No novo painel Filtros, marque ou desmarque os ícones **Bloquear filtro** ou **Ocultar filtro** em um cartão de filtro.

   ![Ocultar ou bloquear filtros](media/power-bi-report-filter-preview/power-bi-filter-lock-hide.png)

À medida que você ativa ou desativa esse novo painel Filtros, pode ver as alterações refletidas no relatório. Filtros ocultos não aparecem na janela pop-up de filtro de um visual.

Você também pode configurar o novo painel Filtros para fluir com os indicadores de relatório. Os estados aberto, fechado e de visibilidade do painel podem ser marcados como indicadores.
 
## <a name="format-the-new-filters-pane"></a>Formatar o novo painel Filtros

Uma grande parte dessa nova experiência é que você pode formatar o painel Filtros para combiná-lo com a aparência do relatório. Você pode formatar o painel Filtros de acordo com cada página no relatório. Estes são os elementos que você pode formatar: 

- Cor da tela de fundo
- Transparência da tela de fundo
- Borda ativada ou desativada
- Cor da borda
- Fonte, cor e tamanho do texto do cabeçalho e título

Você também pode formatar esses elementos para cartões de filtro, dependendo se eles forem aplicados (configurados para algo) ou disponíveis (desmarcados): 

- Cor da tela de fundo
- Transparência da tela de fundo
- Borda: ativada ou desativada
- Cor da borda
- Fonte, cor e tamanho do texto
- Cor da caixa de entrada

### <a name="format-the-filters-pane-and-cards"></a>Formatar o painel Filtros e cartões

1. No relatório, clique no próprio relatório ou na tela de fundo (*papel de parede*), em seguida, no painel **Visualizações**, selecione **Formato**. 
    Você verá as opções de formatação da página do relatório, o papel de parede e também o painel Filtros e Cartões de filtro.

    ![Selecionar o ícone Formato](media/power-bi-report-filter-preview/power-bi-filter-format.png)    

1. Expanda o **painel Filtro** para definir a cor do plano de fundo, o ícone e a borda esquerda, a fim de complementar a página do relatório.

    ![Expandir o painel Filtro](media/power-bi-report-filter-preview/power-bi-filter-format-pane-font.png)

1. Expanda **Cartões de filtro** para definir a cor e a borda **Disponível** e **Aplicada**. Se você escolher cores diferentes para os cartões disponível e aplicado, ficará óbvio quais filtros serão aplicados. 
  
    ![Expandir Cartão de filtro](media/power-bi-report-filter-preview/power-bi-filter-format-card-font.png)

## <a name="theming-for-filter-pane"></a>Temas para o painel de filtros
Agora é possível modificar as configurações padrão do painel de filtros com o arquivo de tema. Veja um trecho do tema de exemplo para começar:

 
```
"outspacePane": [{ 

"backgroundColor": {"solid": {"color": "#0000ff"}}, 

"foregroundColor": {"solid": {"color": "#00ff00"}}, 

"transparency": 50, 

"titleSize": 35, 

"headerSize": 8, 

"fontFamily": "Georgia", 

"border": true, 

"borderColor": {"solid": {"color": "#ff0000"}} 

}], 

"filterCard": [ 

{ 

"$id": "Applied", 

"transparency": 0, 

"backgroundColor": {"solid": {"color": "#ff0000"}}, 

"foregroundColor": {"solid": {"color": "#45f442"}}, 

"textSize": 30, 

"fontFamily": "Arial", 

"border": true, 

"borderColor": {"solid": {"color": "#ffffff"}}, 

"inputBoxColor": {"solid": {"color": "#C8C8C8"}} 

}, 

{ 

"$id": "Available", 

"transparency": 40, 

"backgroundColor": {"solid": {"color": "#00ff00"}}, 

"foregroundColor": {"solid": {"color": "#ffffff"}}, 

"textSize": 10, 

"fontFamily": "Times New Roman", 

"border": true, 

"borderColor": {"solid": {"color": "#123456"}}, 

"inputBoxColor": {"solid": {"color": "#777777"}} 

}] 
```

## <a name="sort-the-filter-pane"></a>Classificar o painel de filtros

A funcionalidade de classificação personalizada é parte da nova experiência de painel de filtros. Os criadores de relatório podem arrastar e soltar os filtros para reorganizá-los na ordem desejada.

![Reorganizar a ordem de classificação de filtros](media/power-bi-report-filter-preview/power-bi-filter-sort.gif)

A ordem de classificação padrão é alfabética para filtros. Para iniciar o modo de classificação personalizada, basta arrastar qualquer filtro para uma nova posição. Você só pode classificar os filtros no nível ao qual eles se aplicam, por exemplo, um filtro no nível visual, no nível da página ou no nível do relatório.

## <a name="filters-pane-scaling"></a>Dimensionamento do painel Filtros

O novo painel Filtros pode ser dimensionado com a página de relatório e visuais, portanto, a página de relatório e o painel Filtros permanecem em proporção um com o outro.

## <a name="improved-filters-pane-accessibility"></a>Acessibilidade aprimorada do painel Filtros

Melhoramos a navegação de teclado para o novo painel Filtros. Você pode percorrer todas as partes do painel Filtros e usar a chave de contexto no teclado ou Shift+F10 para abrir o menu de contexto.

![Acessibilidade do painel Filtros](media/power-bi-report-filter-preview/power-bi-filter-accessible.png)

## <a name="rename-filters"></a>Renomear filtros
Quando você está editando o painel Filtros, pode dar um clique duplo no título para editá-lo. Renomear é útil se você quiser atualizar o cartão de filtro para fazer mais sentido para seus usuários finais. Lembre-se de que renomear o cartão de filtro faz *não* renomear o nome de exibição do campo na lista de campos. Apenas altera o nome de exibição usado no cartão de filtro.

![Renomear um filtro](media/power-bi-report-filter-preview/power-bi-filter-rename.png)

## <a name="restrict-changes-to-filter-type"></a>Restringir alterações para o tipo de filtro

Na seção Experiência de filtragem das configurações de relatório há uma opção para controlar se os usuários podem alterar o tipo de filtro.

![Restringir a forma de alteração para o tipo de filtro](media/power-bi-report-filter-preview/power-bi-filter-restrict-change.png)

## <a name="next-steps"></a>Próximas etapas

Experimente a nova experiência de filtro. Forneça seus comentários sobre esse recurso e como podemos continuar melhorando, [no site Power BI Ideas](https://ideas.powerbi.com/forums/265200-power-bi). 

- [Como usar filtros de relatório](consumer/end-user-report-filter.md)
- [Filtros e realce em relatórios](power-bi-reports-filters-and-highlighting.md)
- [Diferentes tipos de filtros no Power BI](power-bi-report-filter-types.md)

Mais perguntas? [Experimente a Comunidade do Power BI](http://community.powerbi.com/)

