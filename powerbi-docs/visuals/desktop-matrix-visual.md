---
title: Usar o visual de matriz no Power BI
description: Saiba como o visual de matriz permite layouts de nível e realce granular no Power BI.
author: mihart
manager: kvivek
ms.reviewer: ''
ms.service: powerbi
ms.subservice: powerbi-desktop
ms.topic: conceptual
ms.date: 06/25/2019
ms.author: mihart
LocalizationGroup: Visualizations
ms.openlocfilehash: 2f50a6fc9fccc35333257caaf3efeb8185c8caff
ms.sourcegitcommit: 1c96b65a03ec0a0612e851dd58c363f4d56bca38
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2019
ms.locfileid: "67390378"
---
# <a name="use-the-matrix-visual-in-power-bi"></a>Usar o visual de Matriz no Power BI
O visual **matriz** é semelhante a uma **tabela**.  Uma tabela dá suporte a duas dimensões e os dados são simples, o que significa que os valores duplicados são exibidos e não agregados. Uma matriz facilita significativamente a exibição dos dados entre várias dimensões – ela dá suporte a um layout em níveis. A matriz agrega automaticamente os dados e permite fazer drill down. 

Você pode criar visuais de matriz em relatórios do **Power BI Desktop** e **serviço do Power BI**, além de fazer realce cruzado de elementos na matriz com outros visuais na página desse relatório. Por exemplo, é possível selecionar linhas, colunas e até mesmo células individuais e fazer o realce cruzado. Além disso, células individuais e seleções de várias célula podem ser copiadas e coladas em outros aplicativos. 

![matriz com realce cruzado e gráfico de rosca](media/desktop-matrix-visual/matrix-visual_2a.png)

Há muitos recursos associados à matriz e vamos abordá-los nas próximas seções deste artigo.


## <a name="understanding-how-power-bi-calculates-totals"></a>Noções básicas sobre como o Power BI calcula totais

Antes de aprender a usar o elemento visual **Matriz**, é importante saber como o Power BI calcula valores totais e subtotais em tabelas e matrizes. Para linhas de totais e subtotais, o Power BI avalia a medida sobre todas as linhas nos dados subjacentes – não se trata de uma simples adição dos valores nas linhas visíveis ou exibidas. Isso significa que você pode acabar com valores diferentes na linha de total do que o esperado.

Dê uma olhada nos seguintes visuais de matriz. 

![compara tabela e matriz](media/desktop-matrix-visual/matrix-visual_3.png)

Neste exemplo, cada linha no visual de matriz na extrema direita está mostrando a *quantidade* de cada combinação de vendedor/data. No entanto, como um vendedor aparece em várias datas, os números podem aparecer mais de uma vez. Assim, o total preciso dos dados subjacentes e uma simples adição de valores visíveis não são iguais. Este é um padrão comum quando o valor que você está somando está no lado 'um' de uma relação de um para muitos.

Ao examinar totais e subtotais, lembre-se de que esses valores são baseados nos dados subjacentes. Eles não se baseiam exclusivamente nos valores visíveis.

<!-- use Nov blog post video

## Expanding and collapsing row headers
There are two ways you can expand row headers. The first is through the right-click menu. You’ll see options to expand the specific row header you clicked on, the entire level or everything down to the very last level of the hierarchy. You have similar options for collapsing row headers as well.

![](media/desktop-matrix-visual/power-bi-expand1.png)

You can also add +/- buttons to the row headers through the formatting pane under the row headers card. By default, the icons will match the formatting of the row header, but you can customize the icons’ color and size separately if you want. 
Once the icons are turned on, they work similarly to the icons from PivotTables in Excel.

![](media/desktop-matrix-visual/power-bi-expand2.png)

The expansion state of the matrix will save with your report. It can be pinned to dashboards as well, but consumers will need to open up the report to change the state. Conditional formatting will only apply to the inner most visible level of the hierarchy. Note that this expand/collapse experience is not currently supported when connecting to AS servers older than 2016 or MD servers.

![](media/desktop-matrix-visual/power-bi-expand3.png)

Watch the following video to learn more about expand/collapse in the matrix:

-->
## <a name="using-drill-down-with-the-matrix-visual"></a>Como usar drill down com o visual de matriz
Com o visual de matriz, é possível realizar todos os tipos de atividade de drill down interessantes que antes não estavam disponíveis. Isso inclui a capacidade de fazer drill down usando linhas, colunas e até mesmo células e seções individuais. Vamos dar uma olhada em como cada uma delas funciona.

### <a name="drill-down-on-row-headers"></a>Drill down nos cabeçalhos de linha

No painel Visualizações, ao adicionar vários campos à seção **Linhas** do espaço **Campos**, você habilita o drill down nas linhas do visual de matriz. Isso é semelhante à criação de uma hierarquia, o que permite fazer drill down (e, em seguida, drill up) nessa hierarquia e analisar os dados em cada nível.

Na imagem a seguir, a seção **Linhas** contém *Estágio da venda* e *Tamanho da oportunidade*, criando um agrupamento (ou uma hierarquia) nas linhas que podemos detalhar.

![Cartão de filtros mostrando as linhas escolhidas](media/desktop-matrix-visual/power-bi-rows-matrix.png)

Quando o visual tiver algum agrupamento criado na seção **Linhas**, o próprio visual exibirá os ícones *analisar* e *expandir* no canto superior esquerdo do visual.

![matriz com controles de análise destacados](media/desktop-matrix-visual/power-bi-matrix-drilldown.png)

Semelhante ao comportamento de analisar e expandir nos outros visuais, selecionar esses botões permite fazer drill down (ou drill up) na hierarquia. Nesse caso, podemos fazer drill down de *Estágio da venda* para *Tamanho da oportunidade*, conforme mostra a imagem a seguir, em que o ícone de fazer drill down de um nível (a forquilha) foi selecionado.

![matriz com pitchfork contornado](media/desktop-matrix-visual/power-bi-matrix-drill3.png)

Além de usar esses ícones, você pode selecionar qualquer um desses cabeçalhos de linha e fazer drill down escolhendo no menu que é exibido.

![opções de menu para linhas na matriz](media/desktop-matrix-visual/power-bi-matrix-menu.png)

Observe que há algumas opções no menu que aparece, que geram resultados diferentes:

Selecionar **Fazer Drill Down** expande a matriz no nível *dessa* linha, *excluindo* todos os outros cabeçalhos de linha, exceto o cabeçalho de linha que foi selecionado. Na imagem a seguir **Proposta** > **Fazer Drill Down** foi selecionado. Observe que as outras linhas de nível superior não aparecem mais na matriz. Essa maneira de analisar é um recurso útil que fica ainda mais interessante quando chegamos à seção de **realce cruzado**.

![matriz detalhada em um nível](media/desktop-matrix-visual/power-bi-drill-down-matrix.png)

Selecione o ícone **Fazer drill up** para voltar à exibição de nível superior anterior. Se, em seguida, você selecionar **Proposta** > **Mostrar o Próximo Nível**, será exibida uma listagem em ordem crescente de todos os itens do próximo nível (nesse caso, o campo *Tamanho da oportunidade*), sem a categorização de hierarquia de nível superior.

![matriz usando Mostrar o próximo nível](media/desktop-matrix-visual/power-bi-next-level-matrix.png)

Selecione o ícone **Fazer drill up** no canto superior esquerdo para que a matriz mostre todas as categorias de nível superior. Em seguida, selecione **Proposta** > **Expandir para o próximo nível** para ver todos os valores de ambos os níveis da hierarquia – *Estágio da venda* e *Tamanho da oportunidade*.

![matriz usando Expandir para o próximo nível](media/desktop-matrix-visual/power-bi-matrix-expand-next.png)

Você também pode usar o item de menu **Expandir** para controlar ainda mais a exibição.  Por exemplo, selecione **Proposta** > **Expandir** > **Seleção**. O Power BI exibe uma linha de total para cada *Estágio da venda* e todas as opões de *Tamanho da oportunidade* para *Proposta*.

![Matriz depois que Expandir é aplicada à Proposta](media/desktop-matrix-visual/power-bi-matrix-expand.png)

### <a name="drill-down-on-column-headers"></a>Drill down nos cabeçalhos de coluna
Semelhante à capacidade de fazer drill down em linhas, também é possível fazer drill down em **colunas**. Na imagem a seguir, há dois campos no espaço do campo **Colunas**, criando uma hierarquia semelhante à que já usamos para as linhas anteriormente neste artigo. No espaço do campo **Colunas**, temos *Região* e *Segmento*. Assim que o segundo campo foi adicionado a **Colunas**, um novo menu suspenso foi exibido no visual; atualmente, ele mostra **Linhas**.

![Matriz após adição do segundo valor de coluna](media/desktop-matrix-visual/power-bi-matrix-row.png)

Para fazer drill down em colunas, selecione **Colunas** no menu *Fazer drill on*, que pode ser encontrado no canto superior esquerdo da matriz. Selecione a região *Leste* e escolha **Fazer Drill Down**.

![menu para drill down de colunas](media/desktop-matrix-visual/power-bi-matrix-column.png)

Quando você seleciona **Fazer Drill Down**, o próximo nível da hierarquia de coluna para *Região > Leste* é exibido, que, nesse caso, é *Contagem da oportunidade*. A outra região é exibida, mas fica esmaecida.

![matriz com drill down de coluna em um nível](media/desktop-matrix-visual/power-bi-matrix-column-drill.png)

O restante dos itens do menu funcionam nas colunas da mesma maneira que nas linhas (veja a seção anterior, **Fazer drill down nos cabeçalhos de linha**). Você pode **Mostrar o Próximo Nível** e **Expandir para o próximo nível** com colunas assim como faz com as linhas.

> [!NOTE]
> Os ícones de drill up e drill down no canto superior esquerdo do visual de matriz aplicam-se apenas a linhas. Para fazer drill down nas colunas, você deve usar o menu acionado com um clique com o botão direito do mouse.

## <a name="stepped-layout-with-matrix-visuals"></a>Layout de nível com visuais de matriz

O visual **Matriz** recua automaticamente as subcategorias em uma hierarquia abaixo de cada pai, chamado de **Layout de nível**.

Na versão original do visual de matriz, as subcategorias eram mostradas em uma coluna inteiramente diferente, ocupando muito mais espaço no visual. A imagem a seguir mostra a tabela no visual de **Matriz** original. Observe as subcategorias em uma coluna separada.

![Captura de tela do visual Matriz antigo mostrando as subcategorias em uma coluna separada.](media/desktop-matrix-visual/matrix-visual_14.png)

Na imagem a seguir, há um visual **Matriz** com o **Layout de nível** em ação. Observe que a categoria *Computadores* tem suas subcategorias (Acessórios de Computadores, Desktops, Laptops, Monitores e assim por diante) ligeiramente recuadas, fornecendo um visual mais limpo e muito mais compacto.

![maneira atual de como essa matriz formata dados](media/desktop-matrix-visual/matrix-visual_13.png)

Você pode ajustar facilmente as configurações do layout de nível. Com o visual **Matriz** selecionado, na seção **Formatar** (o ícone de rolo de pintura) do painel **Visualizações**, expanda a seção **Cabeçalhos de linha**. Você tem duas opções: a opção (que habilita ou desabilita) **Layout de nível** e o **Recuo do layout de nível** (especifica a quantidade de recuo, em pixels).

![Cartão de cabeçalhos de linha exibindo controle de Layout de nível](media/desktop-matrix-visual/power-bi-stepped-matrix.png)

Se você desativar o **Layout de nível**, o Power BI mostrará as subcategorias em outra coluna em vez de recuadas abaixo da categoria pai.

## <a name="subtotals-with-matrix-visuals"></a>Subtotais com visuais de matriz

Ative ou desative os subtotais em visuais de matriz, linhas e colunas. Na imagem a seguir, você pode ver que os subtotais da linha estão definidos como **Ativados**.

![matriz mostrando totais e subtotais](media/desktop-matrix-visual/matrix-visual_20.png)

Na seção **Formato** do painel **Visualizações**, expanda o cartão **Subtotais** e defina o controle deslizante **Subtotais da Linha** como **Desativado**. Quando você fizer isso, os subtotais não serão mostrados.

![matriz com subtotais desativados](media/desktop-matrix-visual/matrix-visual_21.png)

O mesmo processo se aplica aos subtotais da coluna.

## <a name="cross-highlighting-with-matrix-visuals"></a>Realce cruzado com visuais de matriz

Com o visual **Matriz**, você pode selecionar os elementos na matriz como a base para o realce cruzado. Selecione uma coluna em uma **Matriz** e o Power BI realça a coluna, como em outros visuais na página do relatório. Esse tipo de destaque cruzado era um recurso comum de outros visuais e seleções de ponto de dados, então agora o visual **Matriz** oferece a mesma função.

Além disso, usar Ctrl + clique também funciona para o realce cruzado. Por exemplo, na imagem a seguir, uma coleção de subcategorias foi selecionada no visual **Matriz**. Observe como os itens que não foram selecionados no visual estão esmaecidos e como os outros visuais na página refletem as seleções feitas no visual **Matriz**.

![Captura de tela do visual Matriz com dois outros visuais demonstrando a função Ctrl+clique para realce cruzado.](media/desktop-matrix-visual/matrix-visual_16.png)

## <a name="copying-values-from-power-bi-for-use-in-other-applications"></a>Copiar valores do Power BI para uso em outros aplicativos

Sua matriz ou tabela pode ter conteúdo que você deseja usar em outros aplicativos: Dynamics CRM, Excel e outros relatórios do Power BI. Clicando com o botão direito do mouse no Power BI, é possível copiar uma única célula ou uma seleção de células na área de transferência. Em seguida, cole-as em outro aplicativo.



* Para copiar o valor de uma única célula, selecione-a, clique com o botão direito do mouse e escolha **Copiar valor**. Com o valor de célula não formatado em sua área de transferência, agora é possível colá-lo em outro aplicativo.

    ![Captura de tela do visual Matriz com uma seta apontando para um valor e o menu de contexto expandido com as opções Copiar valor e Copiar seleção dentro do contorno.](media/desktop-matrix-visual/power-bi-cell-copy.png)



* Para copiar mais de uma única célula, selecione uma variedade de células ou use CTRL para selecionar uma ou mais células. 

    ![Captura de tela do visual Matriz com uma seta a partir de três valores realçados apontando na direção do menu de contexto expandido com as opções Copiar valor e Copiar seleção destacadas.](media/desktop-matrix-visual/power-bi-copy.png)

* A cópia incluirá os cabeçalhos da coluna e da linha.

    ![Captura de tela mostrando linhas e colunas do Excel com os valores colados nelas.](media/desktop-matrix-visual/power-bi-copy-selection.png)

## <a name="shading-and-font-colors-with-matrix-visuals"></a>Sombreamento e cores da fonte com visuais de matriz
Com o visual de matriz, você pode aplicar **Formatação condicional** (cores e sombreamento e barras de dados) ao plano de fundo das células na matriz, bem como pode aplicar formatação condicional aos próprios valores e texto.

Para aplicar a formatação condicional, selecione o visual de matriz e abra o painel **Formatar**. Expanda o cartão **Formatação condicional** e para **Cor do plano de fundo**, **Cor da fonte** ou **Barras de dados**, mova o controle deslizante para **Ativado**. A ativação de uma dessas opções exibe um link para *Controles avançados*, que permite personalizar as cores e os valores da formatação de cor.
  
  ![Painel Formatar mostrando controle de Barras de dados](media/desktop-matrix-visual/power-bi-matrix-data-bars.png)

Selecione *Controles avançados* para exibir uma caixa de diálogo que permite fazer ajustes. Este exemplo mostra a caixa de diálogo **Barras de dados**.

![Painel das barras de dados](media/desktop-matrix-visual/power-bi-data-bars.png)

## <a name="next-steps"></a>Próximas etapas

[Gráficos de dispersão e bolhas no Power BI](power-bi-visualization-scatter.md)

[Tipos de visualização no Power BI](power-bi-visualization-types-for-reports-and-q-and-a.md)