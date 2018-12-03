---
title: Usando colunas calculadas no Power BI Desktop
description: Colunas calculadas no Power BI Desktop
author: davidiseminger
manager: kfile
ms.reviewer: ''
ms.service: powerbi
ms.component: powerbi-desktop
ms.topic: conceptual
ms.date: 11/28/2018
ms.author: davidi
LocalizationGroup: Model your data
ms.openlocfilehash: d875a5cd3ded8769ab3734601bd81cf0f17d7cea
ms.sourcegitcommit: 05303d3e0454f5627eccaa25721b2e0bad2cc781
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/28/2018
ms.locfileid: "52578257"
---
# <a name="using-calculated-columns-in-power-bi-desktop"></a>Usando colunas calculadas no Power BI Desktop
Com as colunas calculadas, você pode adicionar novos dados a uma tabela já presente em seu modelo. Mas em vez de consultar e carregar valores em sua nova coluna por meio de uma fonte de dados, você cria uma fórmula DAX (Data Analysis Expressions) que define os valores da coluna. No Power BI Desktop, colunas calculadas são criadas usando o recurso Nova Coluna na Exibição de Relatório.

Diferentemente das colunas personalizadas criadas como parte de uma consulta pelo uso de “Adicionar Coluna Personalizada” no Editor de Consultas, as colunas calculadas criadas na Exibição de Relatório ou Exibição de Dados são baseadas em dados que você já carregou no modelo. Por exemplo, você poderá concatenar os valores de duas colunas diferentes em duas tabelas diferentes, mas relacionadas, realizar adição ou extrair subcadeias de caracteres.

As colunas calculadas que você cria aparecem na lista Campos assim como qualquer outro campo, mas elas têm um ícone especial mostrando que seus valores são resultado de uma fórmula. Você pode nomear suas colunas como desejar e adicioná-las a uma visualização de relatório, assim como com outros campos.

![](media/desktop-calculated-columns/calccolinpbid_fields.png)

Colunas calculadas calculam os resultados usando [DAX](https://msdn.microsoft.com/library/gg413422.aspx) (Data Analysis Expressions), uma linguagem de fórmula destinada a trabalhar com dados relacionais, como no Power BI Desktop. DAX inclui uma biblioteca de mais de 200 funções, operadores e construtores, fornecendo enorme flexibilidade na criação de fórmulas para calcular os resultados de praticamente qualquer análise de dados exigida. Para saber mais sobre o DAX, consulte a seção “Saiba mais” no final deste artigo.

As fórmulas DAX são semelhantes às fórmulas do Excel. Na verdade, o DAX tem muitas das mesmas funções usadas no Excel. Funções DAX, no entanto, devem trabalhar com dados fracionados interativamente ou filtrados em um relatório, como no Power BI Desktop. Diferentemente do Excel, no qual você pode ter uma fórmula diferente para cada linha em uma tabela, uma fórmula DAX criada para uma nova coluna calculará um resultado para cada linha na tabela. Valores de coluna são recalculados conforme necessário, como quando os dados subjacentes são atualizados e os valores mudaram.

## <a name="lets-look-at-an-example"></a>Vejamos um exemplo
Jeff é um gerente de expedição da Contoso. Ele deseja criar um relatório que mostre o número de remessas para cidades diferentes. Ele tem uma tabela Geography com campos separados para cidade e estado. No entanto, Jeff quer que seus relatórios mostrem cidade e estado como um único valor, na mesma linha. No momento, a tabela Geography de Jeff não tem o campo que ele deseja.

![](media/desktop-calculated-columns/calccolinpbid_cityandstatefields.png)

Porém, com uma coluna calculada, Jeff pode simplesmente juntar ou concatenar as cidades na coluna City com os estados da coluna State.

Jeff clica na tabela Geography e, em seguida, clica em Nova Coluna. Em seguida, ele insere a fórmula DAX a seguir na barra de fórmulas:

![](media/desktop-calculated-columns/calccolinpbid_formula.png)

Essa fórmula simplesmente cria uma nova coluna chamada CityState e, para cada linha na tabela Geography, ela usa os valores da coluna City, adiciona uma vírgula e um espaço e, em seguida, concatena os valores da coluna State.

Agora, Jeff tem o campo desejado.

![](media/desktop-calculated-columns/calccolinpbid_citystatefield.png)

Ele poderá adicionar esse campo à sua tela de relatório juntamente com o número de remessas. Muito rapidamente e com o mínimo de esforço, agora Jeff tem um campo City, State, que ele pode adicionar a qualquer tipo de visualização. Jeff vê que, quando ele cria uma visualização de mapa, o Power BI Desktop sabe até mesmo como ler a os valores de City, State em sua nova coluna.

![](media/desktop-calculated-columns/calccolinpbid_citystatemap.png)

## <a name="learn-more"></a>Saiba mais
Fornecemos aqui apenas uma rápida introdução às colunas calculadas. Não deixe de consultar o [Tutorial: Criar colunas calculadas no Power BI Desktop](desktop-tutorial-create-calculated-columns.md), em que você pode baixar um arquivo de exemplo e ver lições passo a passo sobre como criar mais colunas. 

Para saber mais sobre o DAX, consulte [Noções básicas do DAX no Power BI Desktop](desktop-quickstart-learn-dax-basics.md).

Para saber mais sobre as colunas que você cria como parte de uma consulta, consulte a seção “Criar colunas personalizadas” em [Tarefas comuns de consulta no Power BI Desktop.](desktop-common-query-tasks.md)  

