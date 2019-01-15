---
title: Conceitos básicos para designers no serviço do Power BI
description: Workspaces, painéis, relatórios, conjunto de dados e pastas de trabalho do Power BI.
author: maggiesMSFT
manager: kfile
ms.reviewer: ''
featuredvideoid: B2vd4MQrz4M
ms.service: powerbi
ms.subservice: powerbi-service
ms.topic: conceptual
ms.date: 12/18/2018
ms.author: maggies
LocalizationGroup: Get started
ms.openlocfilehash: 487a67f48913ee774904377956eee85ccbae49fc
ms.sourcegitcommit: c8c126c1b2ab4527a16a4fb8f5208e0f7fa5ff5a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2019
ms.locfileid: "54296675"
---
# <a name="basic-concepts-for-designers-in-the-power-bi-service"></a>Conceitos básicos para designers no serviço do Power BI

Este artigo presume que você já [se inscreveu no serviço do Power BI](service-self-service-signup-for-power-bi.md) e [adicionou alguns dados](service-get-data.md). Se você ainda não tiver nenhum dado, tente instalar uma [pacote de conteúdo de exemplo do Power BI](sample-datasets.md#the-power-bi-samples-as-content-packs).

![Tela inicial do serviço do Power BI em um navegador](media/service-basic-concepts/power-bi-home-screen.png)

Aqui estão os elementos que você vê quando abre o serviço do Power BI no navegador:

1. Painel de navegação (navegação esquerda)
2. Iniciador do aplicativo do Office 365
3. Botão Página inicial do Power BI
4. Botões de ícone, incluindo configurações, ajuda e comentários
5. Caixa de pesquisa
6. Blocos de um dashboard favorito
7. Relatórios e dashboards favoritos e frequentes

Nos aprofundaremos nesses recursos mais tarde, mas primeiro vamos examinar alguns conceitos do Power BI.

Ou talvez você queira assistir a este vídeo primeiro antes de ler o restante deste artigo.  Nesse vídeo, Will examina os conceitos básicos e oferece um tour pelo serviço do Power BI.

<iframe width="560" height="315" src="https://www.youtube.com/embed/B2vd4MQrz4M" frameborder="0" allowfullscreen></iframe>


## <a name="power-bi-concepts"></a>Conceitos do Power BI
Os quatro maiores blocos de construção do Power BI são: **_dashboards_**, **_relatórios_**, **_pastas de trabalho_** e **_conjuntos de dados_**. E eles ficam todos organizados em **_workspaces_**. É importante entender os workspaces antes de nos aprofundarmos nos quatro blocos de construção, então, vamos começar com essa parte.

## <a name="workspaces"></a>Workspaces
Workspaces são contêineres para painéis, relatórios, pastas de trabalho e conjunto de dados no Power BI. Há dois tipos de workspaces: *Meu Workspace* e *workspaces de aplicativo*. Então, o que é um *aplicativo*? Um *aplicativo* do Power BI é uma coleção de painéis e relatórios para entregar métricas-chave para sua organização. Aplicativos são interativos, mas não podem ser editados.

- *Meu Workspace* é o workspace pessoal para qualquer cliente do Power BI trabalhar com seu próprio conteúdo. Apenas você tem acesso ao Meu Workspace pertencente a você. Você pode compartilhar painéis e relatórios de Meu Workspace. Se você quer colaborar em painéis e relatórios ou criar um aplicativo, convém trabalhar em um workspace de aplicativo.      
-  *Workspaces do aplicativo* são usados para colaborar e compartilhar conteúdo com colegas. Eles também são os locais nos quais você cria, publica e gerencia aplicativos para sua organização. Imagine-os como áreas de preparo e contêineres para o conteúdo que vai formar um aplicativo do Power BI. Você pode adicionar colegas aos seus workspaces do aplicativo e colaborar em painéis, relatórios, pastas de trabalho e conjunto de dados. Todos os membros do workspace do aplicativo precisam ter licenças do Power BI Pro, mas clientes do aplicativo (os colegas que têm acesso aos aplicativos) não necessariamente precisam de licenças Pro.  

Para saber mais, consulte a seção **Compartilhar seu trabalho** do Sumário, começando com [Como eu devo colaborar e compartilhar painéis e relatórios](service-how-to-collaborate-distribute-dashboards-reports.md)


Agora voltemos aos blocos de construção do Power BI. Você não pode ter painéis ou relatórios sem dados (bem, você até pode ter painéis vazios e relatórios vazios, mas eles não são úteis até que tenham dados), então vamos começar com os **conjuntos de dados**.

## <a name="datasets"></a>Conjuntos de dados
Um *conjunto de dados* é uma coleção de dados que você *importa* ou à qual *se conecta*. O Power BI permite que você se conecte a todos os tipos de conjuntos de dados, os importe e os reúna em um único lugar.  

Conjuntos de dados estão associados aos *workspaces*, e um conjunto de dados exclusivo pode ser parte de muitos workspaces. Ao abrir um workspace, os conjuntos de dados associados estarão listados na guia **Conjuntos de Dados**. Cada conjunto de dados listado representa uma fonte de dados única, por exemplo, uma planilha do Excel no OneDrive, um conjunto de dados de tabela SSAS local ou um conjunto de dados do Salesforce. Há várias diferentes fontes de dados com suporte, e sempre estamos adicionando novas. [Veja a lista de tipos de conjunto de dados que podem ser usados com o Power BI](service-get-data.md).

No exemplo abaixo, selecionamos o workspace do aplicativo “Vendas e marketing” e clicamos na guia para **Conjuntos de dados**.

![Conjuntos de dados estão selecionados](media/service-basic-concepts/power-bi-datasets.png)

**UM** conjunto de dados...

* pode ser usado repetidamente em um ou mais workspaces.
* pode ser usado em vários relatórios diferentes.
* Visualizações desse único conjunto de dados podem ser exibidas em vários painéis diferentes.

  ![Diagrama de conjunto de dados](media/service-basic-concepts/drawing2.png)

Para [conectar-se a um conjunto de dados ou importá-lo](service-get-data.md), selecione **Obter Dados** (na parte inferior da navegação esquerda) ou selecione **+ Criar > Conjunto de dados** (no canto superior direito). Siga as instruções para se conectar à fonte específica ou importá-la e depois adicionar o conjunto de dados ao workspace ativo. Novos conjuntos de dados ficam marcados com um asterisco amarelo. O trabalho que você realiza no Power BI não altera o conjunto de dados subjacente.

Se você fizer [parte de um **_workspace de aplicativo_**](service-collaborate-power-bi-workspace.md), os conjuntos de dados adicionados por um membro do workspace estarão disponíveis para os outros membros do workspace.

Conjuntos de dados podem ser atualizados, renomeados, explorados e removidos. Use um conjunto de dados para criar um relatório do zero ou executando [insights rápidos](service-insights.md).  Para ver quais relatórios e painéis já estão usando um conjunto de dados, selecione **Exibição relacionada**. Para explorar um conjunto de dados, selecione-o. O que você está fazendo é abrir o conjunto de dados no editor de relatórios, onde pode de fato começar a se aprofundar nos dados e criar visualizações. Então, vamos passar para o próximo tópico – relatórios.

### <a name="dig-deeper"></a>Mergulhe mais fundo
* [O que é o Power BI Premium?](service-premium.md)
* [Obter dados para o Power BI](service-get-data.md)
* [Conjuntos de dados de amostra para o Power BI](sample-datasets.md)

## <a name="reports"></a>Relatórios
Um relatório do Power BI é uma ou mais páginas de visualizações como gráficos de linhas, mapas e mapas de árvore. As visualizações também são chamadas de **_visuais_**. Todas as visualizações em um relatório vêm de um único conjunto de dados. Relatórios podem ser criados do zero dentro do Power BI, podem ser importados com painéis que colegas compartilharam com você ou podem ser criados quando você se conectar a conjuntos de dados do Excel, Power BI Desktop, banco de dados, aplicativos SaaS e [aplicativos](service-get-data.md).  Por exemplo, quando você se conecta a uma pasta de trabalho do Excel que contém planilhas do Power View, o Power BI cria um relatório baseado nessas planilhas. E quando você se conecta a um aplicativo SaaS, o Power BI importa um relatório pré-criado.

Há dois modos para exibir e interagir com relatórios: [Modo de Exibição de Leitura e Modo de Exibição de Edição](service-reading-view-and-editing-view.md).  Somente a pessoa que criou o relatório, coproprietários e pessoas com permissão têm acesso a todos os recursos de exploração, criação e compartilhamento do **_Modo de Exibição de Edição_** desse relatório. As pessoas com quem eles compartilham o relatório podem explorar e interagir com o relatório no **_Modo de Exibição de Leitura_**.   

Ao abrir um workspace, os relatórios associados ficam listados na guia **Relatórios**. Cada relatório listado representa uma ou mais páginas de visualizações baseadas em apenas um conjunto de dados subjacente. Para abrir um relatório, selecione-o.

Ao abrir um aplicativo, você verá um painel.  Para acessar um relatório subjacente, selecione um bloco do painel (falaremos mais sobre isso depois) que foi fixado em um relatório. Lembre-se de que nem todos os blocos são fixados em relatórios, então, talvez seja preciso clicar em alguns blocos para encontrar um relatório.

Por padrão, o relatório abre em Modo de Exibição de Leitura.  Basta selecionar **Editar relatório** para abri-lo no Modo de Exibição de Edição (caso tenha as permissões necessárias).

No exemplo abaixo, selecionamos o aplicativo de workspace “Vendas e marketing” e clicamos na guia **Relatórios**.

![Relatórios selecionados](media/service-basic-concepts/power-bi-reports.png)

**UM** relatório...

* está contido em um único workspace.
* pode ser associado com vários painéis dentro desse workspace (blocos fixados a partir desse relatório podem aparecer em diversos painéis).
* pode ser criado usando os dados de um conjunto de dados. (a pequena exceção é que o Power BI Desktop pode combinar mais de um conjunto de dados em um único relatório que pode ser importado no Power BI).

  ![Diagrama de relatórios](media/service-basic-concepts/drawing3new.png)

### <a name="dig-deeper"></a>Mergulhe mais fundo
* [Relatórios no serviço do Power BI e Power BI Desktop](service-reports.md)
* [Relatórios em aplicativos móveis no Power BI](mobile-reports-in-the-mobile-apps.md)

## <a name="dashboards"></a>Dashboards
Um *painel* é algo que você cria **no serviço do Power BI** ou algo que um colega cria **no serviço do Power BI** e compartilha com você. Trata-se de uma única tela, que contém nenhum ou mais blocos e widgets. Cada bloco fixado em um relatório ou uma [P e R](power-bi-q-and-a.md) exibe uma única [visualização](power-bi-report-visualizations.md) que foi criada a partir de um conjunto de dados e fixado ao painel. Páginas inteiras do relatório também podem ser fixadas a um painel como um bloco único. Há várias maneiras de adicionar blocos ao seu painel; muitas maneiras para serem abordadas neste tópico de visão geral. Para saber mais, veja [Blocos do painel no Power BI](service-dashboard-tiles.md).

Por que as pessoas criam painéis?  Aqui estão apenas alguns dos motivos:

* para ver rapidamente todas as informações necessárias para tomar decisões.
* para monitorar as informações mais importantes sobre seus negócios.
* para garantir que todos os colegas estejam na mesma página, exibindo e usando as mesmas informações.
* para monitorar a integridade uma empresa, produto, unidade de negócios, campanha de marketing, etc.
* para criar uma exibição personalizada de um dashboard maior – todas as métricas importantes para você.

Ao abrir um workspace, os painéis associados ficam listados na guia **Painéis**. Para abrir um dashboard, selecione-o. Ao abrir um aplicativo, você verá um painel.  Cada painel representa uma exibição personalizada de algum subconjunto dos conjuntos de dados subjacentes.  Se você possui seu próprio painel, também será preciso editar o acesso aos conjuntos de dados e relatórios subjacentes.  Caso o painel tenha sido compartilhado com você, será possível interagir com ele e quaisquer relatórios subjacentes, mas não será possível salvar quaisquer alterações.

Há muitas maneiras diferentes para você ou um colega [compartilhar um painel](service-share-dashboards.md). É preciso ter o Power BI Pro para compartilhar um painel e pode ser necessário para exibir um painel compartilhado.

**UM** painel...

* está associado a um único workspace
* pode exibir visualizações de vários conjuntos de dados diferentes
* pode exibir visualizações de vários relatórios diferentes
* pode exibir visualizações fixadas de outras ferramentas (por exemplo, Excel)

  ![Dashboard selecionado](media/service-basic-concepts/drawing1.png)

### <a name="dig-deeper"></a>Mergulhe mais fundo
* [Criar um novo painel em branco e obter alguns dados](service-dashboard-create.md)
* [Duplicar um painel](service-dashboard-copy.md)
* [Criar um modo de exibição de telefone de um painel](service-create-dashboard-mobile-phone-view.md)


## <a name="workbooks"></a>Pastas de Trabalho
Pastas de Trabalho são um tipo especial de conjunto de dados. Se você leu a seção **Conjuntos de dados** anterior, já deve saber praticamente tudo de que precisa sobre pastas de trabalho. Mas você deve estar se perguntando porque algumas vezes o Power BI classifica uma pasta de trabalho do Excel como um **Conjunto de dados** e outras vezes como uma **Pasta de trabalho**.

Ao usar o **Obter dados** com arquivos de Excel, você tem a opção de *Importar* ou *Conectar-se* ao arquivo. Ao escolher Conectar-se, sua pasta de trabalho vai aparecer no Power BI assim como apareceria no Excel Online. Mas, ao contrário do Excel Online, você terá alguns ótimos recursos para ajudá-lo a fixar elementos de suas planilhas diretamente nos dashboards.

Não é possível editar a pasta de trabalho no Power BI. No entanto, se precisar fazer alterações, clique em Editar e escolha a opção para editar a pasta de trabalho no Excel Online ou abri-la no Excel em seu computador. Todas as alterações feitas são salvas na pasta de trabalho no OneDrive.

### <a name="dig-deeper"></a>Mergulhe mais fundo
* [Obter dados de arquivos de pasta de trabalho do Excel](service-excel-workbook-files.md)
* [Publicar no Power BI com o Excel](service-publish-from-excel.md)


## <a name="a-dashboard-in-my-workspace"></a>Um dashboard em meu workspace
Nós falamos sobre workspaces e blocos de construção. Vamos reuni-los e examinar as partes que compõem a experiência do dashboard no serviço do Power BI.

![Serviço do Power BI em um navegador](media/service-basic-concepts/completenewest.png)

### <a name="1-navigation-pane-left-nav"></a>1. **Painel de navegação** (nav esq)
Use o painel de navegação para localizar e se mover entre os workspaces e os blocos de construção do Power BI: painéis, relatórios, pastas de trabalho e conjuntos de dados.  

  ![Painel de navegação](media/service-basic-concepts/power-bi-navigation.png)

* Selecione **Obter Dados** para [adicionar conjuntos de dados, relatórios e dashboards ao Power BI](service-get-data.md).
* Expanda e recolha o painel de navegação com este ícone ![ícone do painel de navegação](media/service-basic-concepts/expand-icon.png).
* Abra ou gerencie seu conteúdo favorito selecionando **Favoritos**.
* Exiba e abra o conteúdo visitado mais recentemente selecionando **Recente**.
* Exiba, abra ou exclua um aplicativo selecionando **Aplicativos**.
* Algum colega compartilhou um conteúdo com você? Selecione **Compartilhado comigo** para pesquisar e classificar esse conteúdo para encontrar aquilo de que precisa.
* Exiba e abra seus workspaces selecionando **Workspaces**.

Clique uma vez em nesses elementos:

* um ícone ou cabeçalho para abrir a exibição de conteúdo
* uma seta à direita (>) para abrir um menu do submenu para Favoritos, Recentes e Workspaces.
* um ícone de divisa para exibir a lista rolável de dashboards, relatórios, pastas de trabalho e conjuntos de dados do **Meu Workspace**.

### <a name="2-canvas"></a>2. **Telas**
Como abrimos um painel, a área de telas exibe blocos de visualização. Se, por exemplo, nós tivéssemos aberto o editor de relatório, a área de telas exibiria uma página de relatório.

Os painéis são compostos por [blocos](service-dashboard-tiles.md).  Blocos são criados no Modo de Exibição de Edição de relatório, P e R e outros painéis e podem ser fixados no Excel, SSRS e outros. Um tipo especial de bloco chamado de [widget](service-dashboard-add-widget.md) é adicionado diretamente ao painel. Os blocos que aparecem em um painel foram especificamente inseridos ali pelo criador/proprietário de um relatório.  O ato de adicionar um bloco em um painel é chamado *fixação*.

![Telas de painel do Power BI](media/service-basic-concepts/canvas.png)

Para obter mais informações, consulte [Dashboards](#dashboards) (acima).

### <a name="3-qa-question-box"></a>3. **Caixa de perguntas de P e R**
Uma maneira de explorar seus dados é fazer uma pergunta e deixar que o P e R do Power BI lhe forneça uma resposta, na forma de uma visualização. O P e R pode ser usado para adicionar conteúdo a um painel ou relatório.

O P e R procura uma resposta no conjunto(s) de dados conectado ao painel.  Um conjunto de dados conectado é aquele que tem pelo menos um bloco anexado a esse painel.

![caixa de perguntas de P e R](media/service-basic-concepts/power-bi-qna.png)

Assim que você começa a digitar sua pergunta, o P e R leva você até a página de P e R. Conforme você digita, o P e R ajuda você a fazer a pergunta certa e encontrar a melhor resposta com reformulações, preenchimento automático, sugestões e muito mais. Quando você encontrar uma visualização (resposta) de que gosta, fixe-a em seu painel. Para obter mais informações, veja [P e R no Power BI](power-bi-q-and-a.md).

### <a name="4-icon-buttons"></a>4. **Botões de ícone**
Os ícones no canto superior direito são seus recursos para configurações, notificações, downloads, obter ajuda e fornecer comentários à equipe do Power BI. Selecione a seta dupla para abrir o dashboard no modo **Tela inteira**.  

![botões de ícone](media/service-basic-concepts/power-bi-icons.png)

### <a name="5-dashboard-title-navigation-path-aka-breadcrumbs"></a>5. **Bloco do dashboard** (caminho de navegação, também trilhas)
Nem sempre é fácil descobrir quais workspaces e painéis estão ativos, por isso, o Power BI cria um caminho de navegação para você.  Neste exemplo, veremos o workspace (Meu workspace) e o título do dashboard (Exemplo de Análise de Varejo).  Se abrimos um relatório, o nome dele seria acrescentado ao final do caminho de navegação.  Cada seção do caminho é um hiperlink ativo.  

Observe o ícone “C” após o bloco do painel. Esse painel tem uma [marca de classificação de dados](service-data-classification.md) do tipo “confidencial”. A marca identifica o nível de confidencialidade e segurança dos dados. Se o Administrador ativou a classificação de dados, todo painel terá uma definição de marca padrão. Os proprietários de painéis devem mudar a marca para corresponder com o nível de segurança adequado do painel.

![Ícone de classificação de dados](media/service-basic-concepts/power-bi-title.png)

### <a name="6-office-365-app-launcher"></a>6. **Iniciador do aplicativo do Office 365**
Com o iniciador de aplicativos, todos os aplicativos do Office 365 ficam facilmente disponíveis a um clique. Daqui em diante, você pode inicializar rapidamente seus emails, documentos, calendários e muito mais.

![Inicializador de aplicativos do Office](media/service-basic-concepts/power-bi-waffle.png)

### <a name="7-power-bi-home"></a>7. **Página inicial do Power BI**
Selecionar **Power BI** leva você de volta à sua página inicial do Power BI.

   !["Power BI" no serviço](media/service-basic-concepts/version-new.png)

### <a name="8-labeled-icon-buttons"></a>8. **Botões de ícone rotulados**
Essa área da tela contém opções adicionais para interagir com o conteúdo (neste caso, com o painel).  Além dos ícones rotulados que ficam visíveis, ao selecionar as reticências, são reveladas opções para duplicar, imprimir, atualizar o painel e muito mais.

   ![Botões de ícone rotulados](media/service-basic-concepts/power-bi-labeled-icons.png)

## <a name="next-steps"></a>Próximas etapas
- [O que é o Power BI?](power-bi-overview.md)  
- [Navegação: conhecendo o serviço do Power BI](service-the-new-power-bi-experience.md)
- [Vídeos do Power BI](videos.md)  
- [Editor de relatório - faça um tour](service-the-report-editor-take-a-tour.md)

Mais perguntas? [Experimente perguntar à Comunidade do Power BI](http://community.powerbi.com/)
