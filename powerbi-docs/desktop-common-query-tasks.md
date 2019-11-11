---
title: Tarefas comuns de consulta no Power BI Desktop
description: Tarefas comuns de consulta no Power BI Desktop
author: davidiseminger
ms.reviewer: ''
ms.service: powerbi
ms.subservice: powerbi-desktop
ms.topic: conceptual
ms.date: 05/07/2019
ms.author: davidi
LocalizationGroup: Transform and shape data
ms.openlocfilehash: 2b1cf2a7f10fd7249dcdec26b5c5f5d12ff15aca
ms.sourcegitcommit: 64c860fcbf2969bf089cec358331a1fc1e0d39a8
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "73878668"
---
# <a name="common-query-tasks-in-power-bi-desktop"></a>Tarefas comuns de consulta no Power BI Desktop
Ao trabalhar na janela do **Editor de Consultas** do Power BI Desktop, há uma série de tarefas frequentemente usadas. Este documento demonstra as tarefas comuns e fornece links para informações adicionais. 

As tarefas comuns de consulta demonstradas aqui são as seguintes:

* Conectar-se a dados
* Formatar e combinar dados
* Agrupar linhas
* Dinamizar colunas
* Criar colunas personalizadas
* Fórmulas de consulta

Usaremos algumas conexões de dados para concluir essas tarefas. Os dados estão disponíveis para conexão ou download, caso você deseje executar essas tarefas por conta própria.

A primeira conexão de dados é uma pasta de trabalho do Excel, que pode ser baixada [desse link](https://download.microsoft.com/download/5/7/0/5701F78F-C3C2-450C-BCCE-AAB60C31051D/PBI_Edu_ELSi_Enrollment_v2.xlsx). A outra é um recurso da Web (que também é usado em outro conteúdo de ajuda do Power BI Desktop), que pode ser acessado aqui:

[*https://www.bankrate.com/finance/retirement/best-places-retire-how-state-ranks.aspx*](https://www.bankrate.com/finance/retirement/best-places-retire-how-state-ranks.aspx)

É nas etapas necessárias para conectar-se a ambas as fontes de dados que começam as tarefas comuns de Consulta.

## <a name="connect-to-data"></a>Conectar-se a dados
Para se conectar aos dados no Power BI Desktop, selecione o botão **Obter Dados** da guia **Página Inicial** na faixa de opções. O Power BI Desktop apresenta um menu com as fontes de dados mais comuns. Para obter uma lista completa de fontes de dados às quais o Power BI Desktop pode se conectar, selecione o botão **Mais...** na parte inferior do menu. Para obter mais informações, veja [Fontes de dados no Power BI Desktop](https://docs.microsoft.com/power-bi/desktop-data-sources).

![](media/desktop-common-query-tasks/commonquerytasks_getdata.png)

Para começar, selecione **Excel** , navegue até a pasta de trabalho e selecione-a. A Consulta inspeciona a pasta de trabalho e apresenta os dados encontrados na janela **Navegador** .

![](media/desktop-common-query-tasks/commonquerytasks_navigator.png)

Você pode selecionar **Editar** para ajustar ou *formatar* os dados antes de carregá-los no Power BI Desktop. Editar uma consulta antes de carregar é especialmente útil ao trabalhar com grandes conjuntos de dados que você pretende reduzir antes do carregamento. Como desejamos fazer isso, selecionamos **Editar**.

Também é fácil se conectar a diferentes tipos de dados. Também gostaríamos de nos conectar a um recurso da Web. Selecione **Obter Dados \> Mais...** e **Outros \> Web**.

![](media/desktop-common-query-tasks/commonquerytasks_getdata_other.png)

A janela **Da Web** é exibida, em que é possível digitar a URL da página da Web.

![](media/desktop-common-query-tasks/datasources_fromwebbox.png)

Selecione **OK**e, assim como antes, o Power BI Desktop inspeciona a pasta de trabalho e apresenta os dados encontrados na janela **Navegador** .

Outras conexões de dados são semelhantes. Se for necessário autenticar-se para fazer uma conexão de dados, o Power BI Desktop solicitará a você as credenciais apropriadas.

Para ver uma demonstração passo a passo da conexão a dados no Power BI Desktop, veja [Conectar-se a dados no Power BI Desktop](https://docs.microsoft.com/power-bi/desktop-connect-to-data).

## <a name="shape-and-combine-data"></a>Formatar e combinar dados
Você pode facilmente formatar e combinar dados com o Editor de Consultas. Esta seção inclui alguns exemplos de como você pode formatar dados. Para ver uma demonstração mais completa de formatação e combinação de dados, confira **[Formatar e combinar dados no Power BI Desktop](https://docs.microsoft.com/power-bi/desktop-shape-and-combine-data)** .

Na seção anterior, nós nos conectamos a dois conjuntos de dados – uma pasta de trabalho do Excel e um recurso da Web. Quando carregado no Editor de Consultas, vemos o seguinte, com a consulta da página da Web selecionada (obtidas das consultas disponíveis listadas no painel **Consultas** no lado esquerdo da janela do Editor de Consultas).

![](media/desktop-common-query-tasks/commonquerytasks_querypaneloaded.png)

Ao formatar dados, você transforma uma fonte de dados na forma e formato que atendem às suas necessidades. Nesse caso, como não precisamos dessa primeira coluna chamada *Título*, vamos removê-la.

No **Editor de Consultas**, vários comandos podem ser encontrados na faixa de opções e em um menu contextual de atalho. Por exemplo, quando você clica com o botão direito na coluna *Cabeçalho*, o menu exibido permite a remoção dessa coluna. Também seria possível selecionar a coluna e depois selecionar o botão **Remover Colunas** na faixa de opções.

![](media/desktop-common-query-tasks/commonquerytasks_removecolumns.png)

Há muitas outras maneiras de formatar os dados nessa consulta: você poderia remover qualquer número de linhas na parte superior ou inferior, adicionar colunas, dividir colunas, substituir valores e executar outras tarefas de formatação para direcionar o Query Editor a obter os dados do modo que você deseja.

## <a name="group-rows"></a>Agrupar linhas
No Editor de Consultas, você pode agrupar os valores de várias linhas em um único valor. Isso pode ser útil ao resumir o número de produtos oferecidos, o total de vendas ou a contagem de alunos.

Neste exemplo, agrupamos linhas em um conjunto de dados de matrículas acadêmicas. Os dados são de uma pasta de trabalho do Excel e foram formatados para que o Query Editor obtenha apenas as colunas de que precisamos, renomeie a tabela e realize algumas outras transformações.

Vamos ver quantas Entidades (isso inclui distritos educacionais e outras entidades educacionais, como distritos de serviços regionais, e assim por diante) existem em cada estado. Selecionamos a coluna *Abrev. do Estado* e o botão **Agrupar Por** na guia **Transformar** ou na guia **Página Inicial** da faixa de opções (**Agrupar Por** está disponível em ambas as guias).

![](media/desktop-common-query-tasks/commonquerytasks_groupby.png)

A janela **Agrupar Por...** é exibida. Quando o Editor de Consultas agrupa linhas, ela cria uma nova coluna na qual coloca os resultados de **Agrupar Por** . É possível ajustar a operação **Agrupar Por** das seguintes maneiras:

1. *Agrupar por* – esta é a coluna a ser agrupada; o Editor de Consultas escolhe a coluna selecionada, mas nesta janela você pode alterá-la para qualquer outra coluna na tabela.
2. *Nome da nova coluna* – o Editor de Consultas sugere um nome para a nova coluna com base na operação que ele aplica à coluna que está sendo agrupada, mas você pode nomear a nova coluna como desejar.
3. *Operação* – especifique aqui a operação aplicada pelo Editor de Consultas.
4. *Adicionar agrupamento* e *Adicionar agregação* – estas opções são exibidas após a seleção da opção **Avançado**. Você pode executar operações de agrupamento (ações**Agrupar Por**) em várias colunas e executar várias agregações, todas dentro da janela **Agrupar Por** e todas em uma única operação. O Editor de Consultas cria uma nova coluna (com base em suas seleções nessa janela) que opera em várias colunas. 

Selecione o botão **Adicionar agrupamento** ou **Adicionar agregação** para adicionar mais agrupamentos ou agregações a uma operação **Agrupar por**. É possível remover um agrupamento ou agregação selecionando o ícone **...** e selecionando **Excluir**, portanto, vá em frente, experimente e veja o resultado.
   
   ![](media/desktop-common-query-tasks/commonquerytasks_groupbynumbered.png)

Quando selecionamos **OK**, a Consulta executa a operação **Agrupar Por** e retorna os resultados. Nossa, veja só – Ohio, Texas, Illinois e Califórnia agora têm mais de mil entidades cada uma!

![](media/desktop-common-query-tasks/commonquerytasks_groupedresult.png)

E com o Editor de Consultas, você pode sempre remover a última operação de formatação selecionando o **X** ao lado da etapa recém-concluída. Portanto, vá em frente e experimente, refaça a etapa se você não gostar dos resultados até que o Editor de Consultas formate seus dados do jeito que você deseja.

## <a name="pivot-columns"></a>Dinamizar colunas
Com o Power BI Desktop, é possível dinamizar colunas e criar uma tabela que contém valores agregados para cada valor exclusivo em uma coluna. Por exemplo, se você precisa saber quantos produtos diferentes você tem em cada categoria de produto, é possível criar rapidamente uma tabela que faz exatamente isso.

Vejamos um exemplo. A tabela **Products** a seguir foi formatada para exibir apenas cada produto exclusivo (por nome) e a qual categoria cada produto pertence. Para criar uma nova tabela que mostra uma contagem de produtos para cada categoria (com base na coluna *CategoryName* ), selecione a coluna e selecione **Dinamizar Coluna** na guia **Transformar** da faixa de opções.

![](media/desktop-common-query-tasks/pivotcolumns_pivotbutton.png)

A janela **Dinamizar Coluna** é exibida, permitindo que você saiba quais valores de coluna serão usados para criar novas colunas (1); além disso, ao expandir **Opções avançadas** (2), você pode selecionar a função que será aplicada aos valores agregados (3).

![](media/desktop-common-query-tasks/pivotcolumns_pivotdialog.png)

Ao selecionar **OK**, a Consulta exibe a tabela de acordo com as instruções de transformação fornecidas na janela **Dinamizar Coluna** .

![](media/desktop-common-query-tasks/pivotcolumns_pivotcomplete.png)

## <a name="create-custom-columns"></a>Criar colunas personalizadas
No Editor de Consultas, você pode criar fórmulas personalizadas que operam em várias colunas em sua tabela e, em seguida, colocar os resultados de tais fórmulas em uma nova coluna (personalizada). O Editor de Consultas facilita a criação de colunas personalizadas.

No Editor de Consultas, selecione **Coluna Personalizada** na guia **Adicionar Coluna** da faixa de opções.

![](media/desktop-common-query-tasks/commonquerytasks_customcolumn.png)

A janela a seguir é exibida. No exemplo a seguir, criamos uma coluna personalizada chamada *Percent ELL* que calcula o percentual entre o total de alunos que são ELL (English Language Learners, aprendizes do idioma inglês).

![](media/desktop-common-query-tasks/customcolumn_addcustomcolumndialog.png)

Assim como com qualquer outra etapa aplicada no Editor de Consultas, se a nova coluna personalizada não fornece os dados que você está procurando, basta excluir a etapa da seção **Etapas Aplicadas** do painel **Configurações de Consulta** selecionando o **X** ao lado da etapa **Personalizada Adicionada** .

![](media/desktop-common-query-tasks/customcolumn_addedappliedstep.png)

## <a name="query-formulas"></a>Fórmulas de consulta
Você pode editar as etapas que o Editor de Consultas gera e também criar fórmulas personalizadas, para obter um controle preciso sobre a conexão aos seus dados e sobre sua formatação. Sempre que o Editor de Consultas executar uma ação nos dados, a fórmula associada à ação é exibida na **Barra de Fórmulas**. Para exibir a **Barra de Fórmulas**, marque a caixa de seleção ao lado da **Barra de Fórmulas** na guia **Exibição** da faixa de opções.

![](media/desktop-common-query-tasks/queryformulas_formulabar.png)

Todas as etapas aplicadas de cada consulta são mantidas pelo Editor de Consultas como texto, que você pode exibir ou modificar. É possível exibir ou modificar o texto de qualquer consulta usando o **Editor Avançado**, que é exibido ao selecionar **Editor Avançado** na guia **Exibição** da faixa de opções.

![](media/desktop-common-query-tasks/queryformulas_advancededitorbutton.png)

Veja aqui o **Editor Avançado**, com as etapas de consulta associadas à consulta **USA\_StudentEnrollment** exibida. Essas etapas são criadas na Linguagem de Fórmula do Power Query, frequentemente designada como **M**. Para obter informações, veja [Saiba mais sobre as fórmulas do Power Query](https://support.office.com/article/Learn-about-Power-Query-formulas-6bc50988-022b-4799-a709-f8aafdee2b2f). Para exibir a especificação da linguagem, confira a [Especificação da Linguagem de Fórmula do Microsoft Power Query para Excel](/powerquery-m/excel-workbook).

![](media/desktop-common-query-tasks/queryformulas_advancededitor.png)

O Power BI Desktop fornece um amplo conjunto de categorias de fórmula. Para obter mais informações e uma referência completa de todas as fórmulas do Editor de Consultas, visite [Categorias de fórmula do Power Query](https://support.office.com/article/Power-Query-formula-categories-125024ec-873c-47b9-bdfd-b437f8716819).

As categorias de fórmula do Editor de Consultas são as seguintes:

* Number
  * Constants
  * Information
  * Conversion and formatting
  * Format
  * Rounding
  * Operations
  * Random
  * Trigonometry
  * Bytes
* Text
  * Information
  * Text comparisons
  * Extraction
  * Modification
  * Membership
  * Transformations
* Logical
* Date
* Time
* DateTime
* DateTimeZone
* Duration
* Record
  * Information
  * Transformations
  * Selection
  * Serialization
* List
  * Information
  * Selection
  * Transformation
  * Membership
  * Set operations
  * Ordering
  * Averages
  * Addition
  * Numerics
  * Generators
* Table
  * Table construction
  * Conversions
  * Information
  * Row operations
  * Column operations
  * Membership
* Values
* Arithmetic operations
* Parameter Types
* Metadata
* Accessing data
* URI
* Binary formats
  * Reading numbers
* Binary
* Lines
* Expression
* Function
* Error
* Comparer
* Splitter
* Combiner
* Replacer
* Tipo

## <a name="next-steps"></a>Próximas etapas
Há inúmeras coisas que você pode fazer com o Power BI Desktop. Para obter mais informações sobre seus recursos, consulte as seguintes fontes:

* [O que é o Power BI Desktop?](desktop-what-is-desktop.md)
* [Visão geral de Consulta com o Power BI Desktop](desktop-query-overview.md)
* [Fontes de dados no Power BI Desktop](desktop-data-sources.md)
* [Conectar-se a dados no Power BI Desktop](desktop-connect-to-data.md)
* [Formatar e combinar dados com o Power BI Desktop](desktop-shape-and-combine-data.md)

