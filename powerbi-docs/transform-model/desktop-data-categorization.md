---
title: Categorização de dados no Power BI Desktop
description: Categorização de dados no Power BI Desktop
author: davidiseminger
ms.reviewer: ''
ms.service: powerbi
ms.subservice: powerbi-desktop
ms.topic: conceptual
ms.date: 01/15/2020
ms.author: davidi
LocalizationGroup: Model your data
ms.openlocfilehash: 4ce9946672514d3d3f181c573789b256888a4372
ms.sourcegitcommit: 0e9e211082eca7fd939803e0cd9c6b114af2f90a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "83325841"
---
# <a name="specify-data-categories-in-power-bi-desktop"></a>Especificar categorias de dados no Power BI Desktop
No Power BI Desktop, você pode especificar a *categoria de dados* para uma coluna de modo que o Power BI Desktop saiba como deve tratar seus valores em uma visualização.

Quando Power BI Desktop importa dados, ele obtém outras informações além dos dados em si, como os nomes de tabela e coluna, e se os dados são uma chave primária. Com essas informações, o Power BI Desktop faz algumas suposições sobre como oferecer a você uma boa uma experiência padrão ao criar uma visualização.
Por exemplo, quando uma coluna tem valores numéricos, você provavelmente desejará agregar isso de alguma forma, portanto, o Power BI Desktop a coloca na área **Valores** do painel **Visualizações**. Ou, para uma coluna com valores de data e hora em um gráfico de linhas, o Power BI Desktop pressupõe que você provavelmente a usará como um eixo de hierarquia de tempo.

No entanto, existem alguns casos que são um pouco mais difíceis, como geografia. Considere esta tabela de uma planilha do Excel:

![](media/desktop-data-categorization/datacategorizationtable.png)

O Power BI Desktop deve tratar os códigos na coluna **GeoCode** como uma abreviação para um País ou um Estado dos EUA?  Isso não está claro, porque um código como esse pode significar qualquer uma dessas opções. Por exemplo, AL pode significar Alabama ou Albânia, AR pode significar Arkansas ou Argentina, CA pode significar Califórnia ou no Canadá. Isso faz diferença quando vamos traçar um gráfico de nosso campo GeoCode em um mapa. 

O Power BI Desktop deve mostrar uma imagem do mundo com os países realçados? Ou ele deve mostrar uma imagem da Estados Unidos com os Estados realçados?  Você pode especificar uma categoria de dados para dados exatamente como esses. A categorização de dados refina ainda mais as informações que o Power BI Desktop pode usar para oferecer as melhores visualizações.  

**Para especificar uma categoria de dados**

1. Na Exibição de **Relatório** ou de **Dados**, na lista **Campos**, selecione o campo que você deseja classificar por uma categorização diferente.
2. Na faixa de opções, na área **Propriedades** da guia **Modelagem**, selecione a seta suspensa ao lado de **Categoria de Dados**.  Essa lista mostra as categorias de dados possíveis que você pode escolher para a coluna. Algumas seleções podem ser desabilitadas se não funcionarem com o tipo de dados atual da coluna.  Por exemplo, se uma coluna for um tipo de dados de data ou hora, o Power BI Desktop não permitirá que você escolha categorias de dados geográficos. 
3. Selecione a categoria desejada.

   ![](media/desktop-data-categorization/desktop-data-categorization.png)

Talvez você também esteja interessado em saber mais sobre a [filtragem geográfica para aplicativos móveis do Power BI](desktop-mobile-geofiltering.md).

