---
title: Guia de introdução com propriedades de eixo e formatação de cor
description: Guia de introdução com propriedades de eixo e formatação de cor
author: mihart
ms.reviewer: ''
ms.service: powerbi
ms.subservice: powerbi-desktop
ms.topic: conceptual
ms.date: 08/06/2018
ms.author: mihart
LocalizationGroup: Visualizations
ms.openlocfilehash: a01598bda6520bbf0bf82175ab4256cf7d529e84
ms.sourcegitcommit: 64c860fcbf2969bf089cec358331a1fc1e0d39a8
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "73880694"
---
# <a name="getting-started-with-color-formatting-and-axis-properties"></a>Guia de introdução com propriedades de eixo e formatação de cor
No **Power BI**, altere a cor de série de dados, pontos de dados e até mesmo da tela de fundo das visualizações. Você também pode alterar como os eixos x e y são apresentados, fornecendo a você controle total sobre como seus painéis e relatórios são exibidos.

Para começar, selecione um **Relatório** do painel **Meu Workspace**. Em seguida, na área do menu superior, selecione **Editar Relatório**.  

![](media/service-getting-started-with-color-formatting-and-axis-properties/gettingstartedcolor_1a.png)

Quando você estiver editando um relatório e você tiver uma visualização selecionada, o painel **Visualizações** será exibido, o que permite adicionar ou alterar as visualizações. Diretamente abaixo das visualizações disponíveis há três ícones: o ícone **Campos** (uma pilha de barras), o ícone **Formato** (um rolo de pintura) e o ícone **Análise** (uma lupa). Na imagem abaixo, o ícone **Campos** está selecionado, indicado por uma barra amarela abaixo do ícone.

![](media/service-getting-started-with-color-formatting-and-axis-properties/gettingstartedcolor_2a.png)

Quando você seleciona **Formato**, a área abaixo do ícone exibe as personalizações de cor e eixo disponíveis para a visualização selecionada no momento.  

![](media/service-getting-started-with-color-formatting-and-axis-properties/gettingstartedcolor_3a.png)

Você pode personalizar muitos elementos de cada visualização:

* Legenda
* Eixo X
* Eixo Y
* Cores de dados
* Rótulos de dados
* Formas
* Área de plotagem
* Título
* Tela de fundo
* Fixar proporção
* Borda

> [!NOTE]
>  
> Você não verá todos esses elementos com cada tipo de visualização. A visualização que você selecionar afetará quais personalizações estão disponíveis; por exemplo, você não verá um eixo X se tiver selecionado um gráfico de pizza porque não há eixo x em um gráfico de pizza.

Observe também que, se você não tiver nenhuma visualização selecionada, será exibido **Filtros** em vez dos ícones, o que permite aplicar filtros a todas as visualizações na página.

Vamos mostrar alguns exemplos: um trabalha com cores, o outro alterando as propriedades de um eixo. Aí, você deve estar pronto para personalizar cores, eixos e rótulos o dia inteiro.

## <a name="working-with-colors"></a>Trabalhando com cores

Vamos percorrer as etapas necessárias para personalizar cores em um gráfico.

1. Selecionei um **gráfico de colunas em cluster** da tela de relatório.
2. Em seguida, escolho o ícone **Formato** para mostrar as personalizações disponíveis.
3. Em seguida, seleciono a pequena seta à esquerda da personalização **Cores de Dados** . Isso mostrará como personalizar as Cores de Dados, com opções específicas para a visualização que selecionei.
4. **Cores de Dados** se expande para baixo para mostrar suas personalizações disponíveis.  
   ![](media/service-getting-started-with-color-formatting-and-axis-properties/gettingstartedcolor_4a.png)

Vamos fazer algumas alterações. Posso selecionar a seta para baixo ao lado da cor para fazer alterações em cada série de dados disponíveis. Vou deixar **Custo de vida** em amarelo, **Clima** em laranja e **Bem-estar da comunidade** será verde. A tela a seguir mostra a última etapa, alterando o **Custo de vida**.  

![](media/service-getting-started-with-color-formatting-and-axis-properties/gettingstartedcolor_5a.png)

As alterações são mostradas na imagem abaixo. Uau, esse é um gráfico brilhante. Aqui estão alguns elementos úteis para observar como trabalhar com cores. Os números na lista a seguir também são mostrados na tela seguinte, indicando onde esses elementos úteis podem ser acessados ou alterados.

1. Não gosta das cores? Sem problemas, basta selecionar **Reverter em padrão** e sua seleção é revertida para as configurações padrão. Você pode fazer isso para uma cor ou para a visualização inteira.
2. Quer uma cor que não vê na paleta? Basta selecionar **Cor personalizada**e escolha uma no espectro.  
   ![](media/service-getting-started-with-color-formatting-and-axis-properties/gettingstartedcolor_6a.png)

Não gostou da alteração que acabou de criar? Use **CTRL + Z** para desfazer, exatamente do modo que você está acostumado a fazer.

## <a name="changing-axis-properties"></a>Alterando as propriedades de eixo

Geralmente é útil modificar o eixo X ou Y. Semelhante ao trabalho com cores, você pode modificar um eixo selecionando o ícone de seta para baixo à esquerda do eixo que você deseja alterar, como mostrado na imagem a seguir.  
![](media/service-getting-started-with-color-formatting-and-axis-properties/gettingstartedcolor_7a.png)

Para recolher as opções do **eixo X** , basta selecionar o ícone de seta para cima ao lado do **eixo X**.

Você pode remover os rótulos do eixo X totalmente, alternando para o botão de opção ao lado do **eixo X**. Você pode também optar por ativar ou desativar os títulos dos eixos selecionando o botão de opção ao lado de **Título**.  

Existem todos os tipos de cores para escolher e muitas outras personalizações que você pode aplicar a seus relatórios e painéis do Power BI.

> [!NOTE]
>  
> Essas personalizações de cor, eixo e relacionadas disponíveis quando o ícone **Formato** é selecionado também estão disponíveis no Power BI Desktop.

## <a name="setting-color-from-text-values"></a>Configurando a cor dos valores de texto

A partir da atualização de agosto de 2018 do **Power BI Desktop**, é possível definir cores pelo valor de texto, ou código hexadecimal, para um elemento de relatório específico. Para obter mais informações, consulte [formatação condicional em tabelas](../desktop-conditional-table-formatting.md).


## <a name="next-steps"></a>Próximas etapas
Para obter mais informações, consulte o seguinte artigo:  

* [Dicas e truques para formatação com cores no Power BI](service-tips-and-tricks-for-color-formatting.md)  
* [Formatação condicional em tabelas](../desktop-conditional-table-formatting.md)

