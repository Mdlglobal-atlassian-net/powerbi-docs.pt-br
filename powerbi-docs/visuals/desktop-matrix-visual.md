---
title: Usar o visual de matriz no Power BI Desktop
description: Saiba como o visual de matriz permite layouts de nível e realce granular no Power BI Desktop
author: mihart
manager: kvivek
ms.reviewer: ''
ms.service: powerbi
ms.component: powerbi-desktop
ms.topic: conceptual
ms.date: 10/25/2018
ms.author: mihart
LocalizationGroup: Create reports
ms.openlocfilehash: 96b2fb3cb1558f862c792b3bed77c9f0c2bc61a5
ms.sourcegitcommit: 60fb46b61ac73806987847d9c606993c0e14fb30
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/25/2018
ms.locfileid: "50101360"
---
# <a name="use-the-matrix-visual-in-power-bi-desktop"></a>Usar o visual Matriz no Power BI Desktop
Com o recurso visual **Matriz**, você pode criar visuais de matriz (às vezes mencionados como *tabelas*) nos relatórios do **Power BI Desktop** e **serviço do Power BI** e elementos de realce cruzado na matriz com outros visuais. Além disso, você pode selecionar linhas, colunas e até mesmo células individuais e realce cruzado. As células individuais e várias seleções de célula podem ser copiadas e coladas em outros aplicativos. Por fim, para fazer melhor uso do espaço de layout, o visual de matriz dá suporte a um layout de nível.

![](media/desktop-matrix-visual/matrix-visual_2a.png)

Há muitos recursos associados à matriz e vamos abordá-los nas próximas seções deste artigo.

## <a name="report-themes"></a>Temas de relatórios
Os visuais de matriz e de tabela refletem o estilo (incluindo cores) do **Tema de Relatório** aplicado. Talvez essa não seja as cores que você espera para o seu visual de matriz, que você pode alterar em sua configuração **Tema de Relatório**. Para obter mais informações, consulte [**Usar Temas de Relatório no Power BI Desktop**](../desktop-report-themes.md) para obter informações sobre temas.

## <a name="understanding-how-power-bi-calculates-totals"></a>Noções básicas sobre como o Power BI calcula totais

Antes de ir para como usar o elemento visual **Matriz**, é importante entender como o Power BI calcula valores totais e subtotais em tabelas e matrizes. Para linhas de totais e subtotais, a medida é avaliada em todas as linhas nos dados subjacentes – *não* é apenas uma simples adição dos valores nas linhas visíveis ou exibidas. Isso significa que você pode acabar com valores diferentes na linha de total do que o esperado. 

Observe os seguintes elementos visuais de **Matriz**. 

![](media/desktop-matrix-visual/matrix-visual_3.png)

Neste exemplo, cada linha no elemento visual **Matriz** mais à direita mostra a *Quantidade* para cada combinação de vendedor/data. No entanto, como um vendedor aparece em várias datas, os números podem aparecer mais de uma vez. Assim, o total preciso dos dados subjacentes e uma simples adição de valores visíveis não são iguais. Este é um padrão comum quando o valor que você está somando está no lado 'um' de uma relação de um para muitos.

Ao examinar o total e os subtotais, lembre-se de que esses valores são baseados nos dados subjacentes e não apenas nos valores visíveis. 


## <a name="using-drill-down-with-the-matrix-visual"></a>Usando o drill down com o visual Matriz
Com o visual **Matriz**, é possível fazer todos os tipos de atividades de drill down interessantes que antes não estavam disponíveis. Isso inclui a capacidade de fazer drill down usando linhas, colunas e até mesmo células e seções individuais. Vamos dar uma olhada em como cada uma delas funciona.

### <a name="drill-down-on-row-headers"></a>Drill down nos cabeçalhos de linha
No painel **Visualizações**, ao adicionar vários campos na seção **Linhas** sob **Campos**, você habilita o drill down nas linhas do visual de matriz. Isso é semelhante à criação de uma hierarquia, o que permite fazer drill down (e, em seguida, drill up) nessa hierarquia e analisar os dados em cada nível.

Na imagem a seguir, a seção **Linhas** contém *Categoria* e *Subcategoria*, criando um agrupamento (ou uma hierarquia) nas linhas em que é possível fazer drill down.

![](media/desktop-matrix-visual/matrix-visual_4.png)

Quando o visual tiver algum agrupamento criado na seção **Linhas**, o próprio visual exibirá os ícones *analisar* e *expandir* no canto superior esquerdo do visual.

![](media/desktop-matrix-visual/matrix-visual_5.png)

Semelhante ao comportamento de analisar e expandir nos outros visuais, selecionar esses botões permite fazer drill down (ou drill up) na hierarquia. Nesse caso, podemos fazer drill down de *Categoria* para *Subcategoria*, conforme mostra a imagem a seguir, em que o ícone de fazer drill down de um nível (a forquilha) foi selecionado.

![](media/desktop-matrix-visual/matrix-visual_6.png)

Além de usar esses ícones, você pode clicar com o botão direito do mouse em qualquer um desses cabeçalhos de linha e fazer drill down selecionando no menu que aparece.

![](media/desktop-matrix-visual/matrix-visual_7.png)

Observe que há algumas opções no menu que aparece, que geram resultados diferentes:

Selecionar **Drill Down** expande a matriz no nível *dessa* linha, *excluindo* todos os outros cabeçalhos de linha, exceto o cabeçalho de linha que foi clicado. Na imagem a seguir, *Computadores* foi clicado com o botão direito do mouse e **Drill Down** foi selecionado. Observe que as outras linhas de nível superior não aparecem mais na matriz. Essa maneira de analisar é um recurso útil que fica ainda mais interessante quando chegamos à seção de **realce cruzado**.

![](media/desktop-matrix-visual/matrix-visual_8.png)

Você pode clicar no ícone **Drill up** para voltar à exibição de nível superior anterior. Se, em seguida, você selecionar **Mostrar Próximo Nível** no menu acionado com um clique do botão direito do mouse, verá uma lista alfabética de todos os itens do próximo nível (nesse caso, o campo *Subcategoria*), sem a categorização de hierarquia de nível superior.

![](media/desktop-matrix-visual/matrix-visual_8a.png)

Ao clicar no ícone **Drill up** no canto superior esquerdo para que a matriz mostre todas as categorias de nível superior, clicar com o botão direito do mouse novamente e selecionar **Expandir para o próximo nível**, você poderá ver o seguinte visual.

![](media/desktop-matrix-visual/matrix-visual_9.png)

Você também pode usar os itens de menu **Incluir** e **Excluir** para manter (ou remover, respectivamente) a linha clicada com o botão direito do mouse (e todas as subcategorias) da matriz.

### <a name="drill-down-on-column-headers"></a>Drill down nos cabeçalhos de coluna
Semelhante à capacidade de fazer drill down em Linhas, você pode também pode fazer drill down em **Colunas**. Na imagem a seguir, você pode ver que há dois campos sob o campo **Colunas**, criando uma hierarquia semelhante à que já usamos para as linhas neste artigo. Sob o campo **Colunas**, temos *Classe* e *Cor*.

![](media/desktop-matrix-visual/matrix-visual_10.png)

No visual **Matriz**, ao clicar com o botão direito do mouse em uma coluna, aparece a opção para fazer drill down. Na imagem a seguir, clicamos com o botão direito do mouse em *Deluxe* e selecionamos **Fazer Drill Down**.

![](media/desktop-matrix-visual/matrix-visual_11.png)

Ao selecionar **Drill Down**, o próximo nível da hierarquia de coluna para *Deluxe* será exibido, que nesse caso é *Cor*.

![](media/desktop-matrix-visual/matrix-visual_12.png)

O restante dos itens do menu acionados clicando com o botão direito do mouse funcionam nas Colunas da mesma maneira que nas linhas (Consulte a seção anterior, **Drill down nos cabeçalhos de linha**). Você pode **Mostrar Próximo Nível**, **Expandir para o próximo nível**, **Incluir** ou **Excluir** colunas, como faz com as linhas.

> [!NOTE]
> Os ícones de drill up e drill down no canto superior esquerdo do visual de matriz aplicam-se apenas a linhas. Para fazer drill down nas colunas, você deve usar o menu acionado com um clique com o botão direito do mouse.
> 
> 

## <a name="stepped-layout-with-matrix-visuals"></a>Layout de nível com visuais de matriz
O visual **Matriz** recua automaticamente as subcategorias em uma hierarquia abaixo de cada pai, chamado de **Layout de nível**.

Na versão *original* do visual de matriz, as subcategorias foram mostradas em uma coluna inteiramente diferente, ocupando muito mais espaço no visual. A imagem a seguir mostra a tabela no visual de **Matriz** original. Observe as subcategorias em uma coluna separada.

![](media/desktop-matrix-visual/matrix-visual_14.png)

Na imagem a seguir, há um visual **Matriz** com o **Layout de nível** em ação. Observe que a categoria *Computadores* tem suas subcategorias (Acessórios de Computadores, Desktops, Laptops, Monitores e assim por diante) ligeiramente recuadas, fornecendo um visual mais limpo e muito mais compacto.

![](media/desktop-matrix-visual/matrix-visual_13.png)

Você pode ajustar facilmente as configurações do layout de nível. Com o visual **Matriz** selecionado, na seção **Formatar** (o ícone de rolo de pintura) do painel **Visualizações**, expanda a seção **Cabeçalhos de linha**. Você tem duas opções: a opção (que habilita ou desabilita) **Layout de nível** e o **Recuo do layout de nível** (especifica a quantidade de recuo, em pixels).

![](media/desktop-matrix-visual/matrix-visual_15.png)

Se você desligar **Layout de nível**, as subcategorias serão mostradas em outra coluna em vez de recuadas abaixo da categoria pai.

## <a name="subtotals-with-matrix-visuals"></a>Subtotais com visuais de matriz
Ative ou desative os subtotais em visuais de matriz, linhas e colunas. Na imagem a seguir, veja que os subtotais da linha são definidos como **ativados**.

![](media/desktop-matrix-visual/matrix-visual_20.png)

Na seção **Formato** do painel **Visualizações**, expanda o cartão **Subtotais** e defina o controle deslizante **Subtotais da Linha** como **Desativado**. Quando você fizer isso, os subtotais não serão mostrados.

![](media/desktop-matrix-visual/matrix-visual_21.png)

O mesmo processo se aplica aos subtotais da coluna.

## <a name="cross-highlighting-with-matrix-visuals"></a>Realce cruzado com visuais de matriz
Com o visual **Matriz**, você pode selecionar os elementos na matriz como a base para o realce cruzado. Selecione uma coluna em uma **Matriz** e essa coluna será realçada, assim como quaisquer outros visuais na página do relatório. Esse tipo de destaque cruzado era um recurso comum de outros visuais e seleções de ponto de dados, então agora o visual **Matriz** oferece a mesma função.

Além disso, usar Ctrl + clique também funciona para o realce cruzado. Por exemplo, na imagem a seguir, uma coleção de subcategorias foi selecionada no visual **Matriz**. Observe como os itens que não foram selecionados no visual estão esmaecidos e como os outros visuais na página refletem as seleções feitas no visual **Matriz**.

![](media/desktop-matrix-visual/matrix-visual_16.png)

## <a name="copying-values-from-power-bi-for-use-in-other-applications"></a>Copiar valores do Power BI para uso em outros aplicativos

Sua matriz ou tabela pode ter conteúdo que você gostaria de usar em outros aplicativos, como Dynamics CRM, Excel e até mesmo outros relatórios do Power BI. Clicando com o botão direito do mouse no Power BI, é possível copiar uma única célula ou uma seleção de células em sua área de transferência e colar em outro aplicativo.

![opções de cópia](media/desktop-matrix-visual/power-bi-cell-copy.png)

* Para copiar o valor de uma única célula, selecione-a, clique com o botão direito do mouse e escolha **Copiar valor**. Com o valor de célula não formatado em sua área de transferência, agora é possível colá-lo em outro aplicativo.

    ![opções de cópia](media/desktop-matrix-visual/power-bi-copy.png)

* Para copiar mais de uma única célula, selecione uma variedade de células ou use CTRL para selecionar uma ou mais células. A cópia incluirá os cabeçalhos da coluna e da linha.

    ![colar no Excel](media/desktop-matrix-visual/power-bi-copy-selection.png)

## <a name="shading-and-font-colors-with-matrix-visuals"></a>Sombreamento e cores da fonte com visuais de matriz
Com o visual **Matriz**, você pode aplicar a **formatação condicional** (cores e sombreamento) à tela de fundo das células dentro da matriz e aplicar a formatação condicional ao próprio texto e aos valores.

Para aplicar a formatação condicional, realize uma das seguintes etapas quando um visual de matriz estiver selecionado:

* No painel **Campos**, clique com o botão direito do mouse no Campo e selecione **Formatação condicional** no menu.
  
  ![](media/desktop-matrix-visual/matrix-visual_17.png)
* Se preferir, no painel **Formato**, expanda o cartão **Formatação condicional** e, em **Escalas de cores da tela de fundo** ou **Escalas de cores da fonte**, defina o controle deslizante como **Ativado**. A ativação de uma dessas opções exibe um link para *Controles avançados*, que permite personalizar as cores e os valores da formatação de cores.
  
  ![](media/desktop-matrix-visual/matrix-visual_18.png)

Qualquer uma dessas abordagem atinge o mesmo resultado. A seleção de *Controles avançados* exibe a seguinte caixa de diálogo, que permite fazer ajustes:

![](media/desktop-matrix-visual/matrix-visual_19.png)

## <a name="next-steps"></a>Próximas etapas

[Gráficos de dispersão e bolhas no Power BI](power-bi-visualization-scatter.md)

[Tipos de visualização no Power BI](power-bi-visualization-types-for-reports-and-q-and-a.md)