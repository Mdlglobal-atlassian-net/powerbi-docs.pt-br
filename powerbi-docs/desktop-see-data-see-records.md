---
title: Ver dados e registros em visuais do Power BI Desktop
description: Usar os recursos Ver Dados e Ver Registros do Power BI Desktop para analisar os detalhes
author: davidiseminger
ms.reviewer: ''
ms.service: powerbi
ms.subservice: powerbi-desktop
ms.topic: conceptual
ms.date: 05/08/2019
ms.author: davidi
LocalizationGroup: Learn more
ms.openlocfilehash: 66fe4a9eb109565108cd150369b2260a9d3e1d06
ms.sourcegitcommit: 64c860fcbf2969bf089cec358331a1fc1e0d39a8
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "73877782"
---
# <a name="use-see-data-and-see-records-in-power-bi-desktop"></a>Use Ver Dados e Ver Registros no Power BI Desktop
No **Power BI Desktop**, é possível analisar em detalhes qualquer visualização e ver as representações textuais dos dados subjacentes ou os registros de dados individuais para o visual selecionado. Esses recursos às vezes são chamados de *clickthrough*, *drill-through* ou *drill-through em detalhes*.

É possível usar **Ver Dados** para exibir uma versão textual dos valores usados pela visualização selecionada ou usar **ver Registros** para exibir todos os dados para um registro ou ponto de dados selecionado. 

![Ver dados e Ver relatórios](media/desktop-see-data-see-records/see-data-record.png)

>[!IMPORTANT]
>**Ver Dados** e **Ver Registros** dão suporte apenas aos seguintes tipos de visualização:
>  - Gráfico de barras
>  - Gráfico de colunas
>  - Gráfico de rosca
>  - Mapa coroplético
>  - Funil
>  - Mapear
>  - Gráfico de pizza
>  - Mapa de árvore

## <a name="use-see-data-in-power-bi-desktop"></a>Usar Ver Dados no Power BI Desktop

**Ver Dados** mostra os dados subjacentes a uma visualização. **Ver Dados** aparece na guia **Dados/Analisar** na seção **Ferramentas Visuais** da faixa de opções quando uma visualização está selecionada.

![Ver Dados na faixa de opções](media/desktop-see-data-see-records/see-data1.png)

Também é possível ver os dados clicando com o botão direito do mouse em uma visualização e, em seguida, selecionando **Mostrar Dados** no menu que aparece. Outra alternativa é selecionar **More options** (...) no canto superior direito de uma visualização e, em seguida, **Mostrar Dados**.

![Mostrar Dados com o botão direito](media/desktop-see-data-see-records/see-data2.png)&nbsp;&nbsp;![Mostrar mais opções de Dados](media/desktop-see-data-see-records/see-data3.png)

> [!NOTE]
> É necessário focalizar um ponto de dados no visual para que o menu de clique com o botão direito do mouse fique disponível.

Quando você seleciona **Ver Dados** ou **Mostrar Dados**, a tela do Power BI Desktop exibe a representação visual e textual dos dados. Na *exibição horizontal*, o visual é exibido na metade superior da tela, e os dados são mostrados na metade inferior. 

![exibição horizontal](media/desktop-see-data-see-records/see-data4a.png)

Você pode alternar entre a exibição horizontal e a *exibição vertical* selecionando o ícone no canto superior direito da tela.

![alternância de exibição vertical](media/desktop-see-data-see-records/see-data4.png)

Para retornar ao relatório, selecione **< Voltar ao Relatório** no canto superior esquerdo da tela.

![Voltar ao Relatório](media/desktop-see-data-see-records/see-data5.png)

## <a name="use-see-records-in-power-bi-desktop"></a>Usar Ver Registros no Power BI Desktop

Também é possível enfocar um registro de dados em uma visualização e detalhar os dados atrás dele. Para usar **Ver Registros**, selecione uma visualização, em seguida **Ver Registros** na guia **Dados/Analisar** na seção **Ferramentas Visuais** da faixa de opções e, em seguida, selecione um ponto de dados ou linha na visualização. 

![Consulte Registros na faixa de opções](media/desktop-see-data-see-records/see-record1.png)

> [!NOTE]
> Se o botão **Ver Registros** na faixa de opções estiver desabilitado e esmaecido, isso significará que a visualização selecionada não oferece suporte a **Ver Registros**.

Você pode também clicar com o botão direito em um elemento de dados e selecionar **Ver Registros** no menu que aparece.

![Consulte Registros clicando com o botão direito](media/desktop-see-data-see-records/see-record2.png)

Quando você seleciona **Ver Registros** para um elemento de dados, a tela do Power BI Desktop exibe todos os dados associados ao elemento selecionado. 

![](media/desktop-see-data-see-records/see-record3.png)

Para retornar ao relatório, selecione **< Voltar ao Relatório** no canto superior esquerdo da tela.

![](media/desktop-see-data-see-records/see-record4.png)

> [!NOTE]
>**Ver Registros** tem as seguintes limitações:
> - Você não pode alterar os dados na exibição **Ver Registros** e salvá-los novamente no relatório.
> - Não é possível usar **Ver Registros** quando seu visual usa uma medida calculada.
> - Não é possível usar **Ver Registros** quando você está conectado a um modelo MD (multidimensional) dinâmico.

## <a name="next-steps"></a>Próximas etapas
Há todos os tipos de recursos para gerenciamento de dados e formatação do relatório no **Power BI Desktop**. Confira os seguintes recursos para alguns exemplos:

* [Usar agrupamento e compartimentalização no Power BI Desktop](desktop-grouping-and-binning.md)
* [Usar linhas de grade, ajustar à grade, ordem z, alinhamento e distribuição em relatórios do Power BI Desktop](desktop-gridlines-snap-to-grid.md)

