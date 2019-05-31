---
title: Formatação de tabela condicional no Power BI Desktop
description: Aplicar formatação personalizada a tabelas
author: davidiseminger
manager: kfile
ms.reviewer: ''
ms.service: powerbi
ms.subservice: powerbi-desktop
ms.topic: conceptual
ms.date: 05/07/2019
ms.author: davidi
LocalizationGroup: Create reports
ms.openlocfilehash: e23fd2aca90ee14c2376b0175c7c8b5132cf9a9f
ms.sourcegitcommit: 60dad5aa0d85db790553e537bf8ac34ee3289ba3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/29/2019
ms.locfileid: "66222274"
---
# <a name="conditional-formatting-in-tables"></a>Formatação condicional em tabelas 
Com a formatação condicional para tabelas, você pode especificar cores personalizadas para as células com base nos valores das células ou em outros valores ou campos, inclusive usando cores de gradiente. Também é possível exibir valores de célula com barras de dados. 

Para acessar a formatação condicional, em **Campos** também do painel **Visualizações** no Power BI Desktop, selecione a seta para baixo ao lado do valor em **Valores** que você deseja formatar (ou clique com o botão direito do mouse no campo). Você pode gerenciar somente a formatação condicional para campos na área **Valores** também em **Campos**.

![Menu Formatação condicional](media/desktop-conditional-table-formatting/table-formatting-0-popup-menu.png)

As seções a seguir descrevem cada uma dessas opções de formatação condicional. Uma ou mais opções podem ser combinadas em uma única coluna de tabela.

> [!NOTE]
> Quando aplicada a uma tabela, a formatação condicional substitui quaisquer estilos de tabela personalizados aplicados a células formatadas condicionalmente.

Para remover a formatação condicional de uma visualização, basta clicar com o botão direito do mouse no campo novamente e selecionar **Remover formatação condicional** e o tipo de formatação a ser removida.

![Menu Remover formatação condicional](media/desktop-conditional-table-formatting/table-formatting-1-remove.png)

## <a name="background-color-scales"></a>Escalas de cores da tela de fundo

Selecionar **Formatação condicional** e **Escalas de cor da tela de fundo** exibe a caixa de diálogo a seguir.

![Caixa de diálogo Escalas de cor da tela de fundo](media/desktop-conditional-table-formatting/table-formatting-1-default-dialog.png)

É possível selecionar um campo do modelo de dados para basear as cores definindo **Cor baseada em** nesse campo. Além disso, você pode especificar o tipo de agregação para o campo selecionado com o valor **Resumo**. O campo a ser colorido é especificado no campo **Aplicar cor a**. Assim, você tem o controle. É possível aplicar a formatação condicional a campos de data e de texto, desde que você escolha um valor numérico como a base da formatação.

![Cor baseada em campo](media/desktop-conditional-table-formatting/table-formatting-1-apply-color-to.png)

Para usar valores de cor discretos para intervalos de valor, selecione **Colorir por regras**. Para usar um espectro de cores, deixe **Colorir por regras** desmarcado. 

![Caixa de diálogo Escalas de cor da tela de fundo](media/desktop-conditional-table-formatting/table-formatting-1-color-by-rules-dialog.png)

### <a name="color-by-rules"></a>Colorir segundo regras

Quando você seleciona **Colorir por regras**, é possível inserir um ou mais intervalos de valores, cada um com um conjunto de cores.  Cada intervalo de valor começa com uma condição de *valor If*, uma condição de valor *and* e uma cor.

![Intervalo de valor de Colorir por regras](media/desktop-conditional-table-formatting/table-formatting-1-color-by-rules-if-value.png)

Células de tabela com valores em cada intervalo são preenchidas com determinada cor. Há três regras na figura a seguir.

![Exemplo de Colorir por regras](media/desktop-conditional-table-formatting/table-formatting-1-color-by-rules.png)

A tabela de exemplo agora tem esta aparência:

![Tabela de exemplo com Colorir por regras](media/desktop-conditional-table-formatting/table-formatting-1-color-by-rules-table.png)


### <a name="color-minimum-to-maximum"></a>Valores mínimo e máximo de cor

Você pode configurar os valores *mínimo* e *máximo* e as cores. Se selecionar a caixa **Divergente**, você também poderá configurar um valor opcional para o *Centro*.

![Botão Divergente](media/desktop-conditional-table-formatting/table-formatting-1-diverging.png)

A tabela de exemplo agora tem esta aparência:

![Tabela de exemplo com cores divergentes](media/desktop-conditional-table-formatting/table-formatting-1-diverging-table.png)

## <a name="font-color-scales"></a>Escalas de cores de fonte

Selecionar **Formatação condicional** e **Escalas de cores de fonte** exibe a caixa de diálogo a seguir. Essa caixa de diálogo é semelhante a **Escalas de cor da tela de fundo**, mas altera a cor da fonte em vez da cor da tela de fundo da célula.

![Caixa de diálogo Escalas de cores de fonte](media/desktop-conditional-table-formatting/table-formatting-2-diverging.png)

A tabela de exemplo agora tem esta aparência:

![Tabela de exemplo com escalas de cores de fonte](media/desktop-conditional-table-formatting/table-formatting-2-table.png)

## <a name="data-bars"></a>Barras de dados

Selecionar **Formatação condicional** e **Barras de dados** exibe a caixa de diálogo a seguir. 

![Caixa de diálogo Barras de dados](media/desktop-conditional-table-formatting/table-formatting-3-default.png)

Por padrão, a opção **Mostrar somente a barra** é desmarcada e, portanto, a célula da tabela mostra a barra e o valor real.

![Tabela de exemplo com barras de dados e valores](media/desktop-conditional-table-formatting/table-formatting-3-default-table.png)

Se opção **Mostrar somente a barra** estiver marcada, a célula da tabela mostrará apenas a barra.

![Tabela de exemplo com apenas as barras de dados](media/desktop-conditional-table-formatting/table-formatting-3-default-table-bars.png)

## <a name="color-formatting-by-field-value"></a>Formatação de cor por valor de campo

É possível usar uma medida ou uma coluna que especifica uma cor, usando um valor de texto ou um código hexadecimal, para aplicar essa cor à tela de fundo da cor da fonte de um visual de tabela ou de matriz. Também é possível criar uma lógica personalizada para um determinado campo e fazer essa lógica aplicar a cor desejada à fonte ou tela de fundo.

Por exemplo, na tabela a seguir, há uma cor associada a cada modelo de produto. 

![Campo ProductName com nome de cor](media/desktop-conditional-table-formatting/conditional-table-formatting_01.png)

Para formatar essa célula com base em seu valor de campo, selecione a caixa de diálogo **Formatação condicional** clicando com o botão direito do mouse na coluna *Cor* desse visual e, nesse caso, selecione **Cor da tela de fundo** no menu. 

![Selecionar a cor da tela de fundo do menu](media/desktop-conditional-table-formatting/conditional-table-formatting_02.png)

Na caixa de diálogo exibida, selecione **Valor do campo** na área suspensa **Formatar por**, conforme mostrado na imagem a seguir.

![Formatar por valor Campo](media/desktop-conditional-table-formatting/conditional-table-formatting_03.png)

É possível repetir esse processo para a cor da fonte, e o resultado no visual será uma cor sólida na coluna **cor**, conforme mostrado na tela a seguir.

![Formatar por valor Campo](media/desktop-conditional-table-formatting/conditional-table-formatting_04.png)

Também é possível criar um cálculo de DAX com base na lógica de negócios, que gera códigos hexadecimais diferentes com base nas condições de sua preferência. Geralmente isso é mais fácil do que criar várias regras na caixa de diálogo de formatação condicional. Considere o campo *ColorKPI* na imagem de exemplo a seguir.

![Cálculos DAX](media/desktop-conditional-table-formatting/conditional-table-formatting_05.png)

Depois é possível definir o valor do campo para **Cor da tela de fundo** da seguinte maneira.

![Definir a cor do campo com base em um KPI](media/desktop-conditional-table-formatting/conditional-table-formatting_06.png)

E, em seguida, é possível obter resultados como a matriz a seguir.

![Visual de matriz com uma cor baseada em um valor de KPI](media/desktop-conditional-table-formatting/conditional-table-formatting_07.png)

Há muito mais variações que você pode criar apenas usando sua imaginação e um pouco do DAX.

Você pode usar qualquer um dos valores listados na especificação de cor CSS no [ https://www.w3.org/TR/css-color-3/ ](https://www.w3.org/TR/css-color-3/) para colorir os elementos visuais:
* 3, 6 ou 8 hex de dígito códigos, por exemplo, #3E4AFF. Certifique-se de que incluir o símbolo # no início do código. "3E4AFF" não é aceito. 
* Por exemplo, RGBA (234, 234, 234, 0,5) de valores de RGB ou RGBA
* HSL ou HSLA, por exemplo, valores HSLA (123, 75%, 75%, 0,5)
* Por exemplo, nas cores verde, SkyBlue, PeachPuff de nomes de cor 

## <a name="next-steps"></a>Próximas etapas
Para obter mais informações, consulte o seguinte artigo:  

* [Dicas e truques para formatação com cores no Power BI](visuals/service-tips-and-tricks-for-color-formatting.md)  

