---
title: Fontes de dados no Power BI Desktop
description: Fontes de dados no Power BI Desktop
author: davidiseminger
manager: kfile
ms.reviewer: ''
ms.service: powerbi
ms.subservice: powerbi-desktop
ms.topic: conceptual
ms.date: 06/10/2019
ms.author: davidi
LocalizationGroup: Connect to data
ms.openlocfilehash: b689a4d0718c92608fe7fc0cdb34d27803015269
ms.sourcegitcommit: e48ef4c88e4a1a0b259bf899d85d520c4edd5751
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2019
ms.locfileid: "66823549"
---
# <a name="data-sources-in-power-bi-desktop"></a>Fontes de dados no Power BI Desktop
O Power BI Desktop permite se conectar a dados de várias fontes diferentes. Veja uma lista completa das fontes de dados disponíveis na parte inferior desta página.

Para se conectar a dados, selecione **Obter Dados** na faixa de opções **Página Inicial** . Selecionar a seta para baixo ou o texto **Obter Dados** no botão exibe o menu de tipos de dados **Mais Comuns** mostrado na imagem a seguir:

![Obter Dados no Power BI Desktop](media/desktop-data-sources/data-sources_01.png)

Selecionar **Mais...** no menu **Mais Comuns** exibe a janela **Obter Dados**. Você também pode abrir a janela **Obter Dados** (e ignorar o menu **Mais Comuns** ) selecionando diretamente o **botão do ícone** **Obter Dados** .

![Botão Obter Dados](media/desktop-data-sources/data-sources_02.png)

> [!NOTE]
> A equipe do Power BI está sempre expandindo as fontes de dados disponíveis para o **Power BI Desktop** e o **serviço do Power BI**. Assim, você verá com frequência as versões anteriores das fontes de dados de trabalho em andamento marcadas como *Beta* ou *Visualização*. Toda fonte de dados marcada como *Beta* ou *Visualização* tem suporte e funcionalidade limitados e não deve ser usada em ambientes de produção.

## <a name="data-sources"></a>Fontes de Dados
Tipos de dados são organizados nas categorias a seguir:

* Todos
* Arquivo
* Banco de dados
* Power BI
* Azure
* Serviços online
* Outros

A categoria **Todos** inclui todos os tipos de conexão de dados de todas as categorias.

A categoria **Arquivo** fornece as seguintes conexões de dados:

* Excel
* Texto/CSV
* XML
* JSON
* Pasta
* PDF
* Pasta do SharePoint

A imagem a seguir mostra a janela **Obter Dados** para **Arquivo**.

![Obter Dados > Arquivo](media/desktop-data-sources/data-sources_03.png)

A categoria **Banco de dados** fornece as seguintes conexões de dados:

* Banco de dados do SQL Server
* Banco de dados do Access
* Banco de dados do SQL Server Analysis Services
* Banco de dados Oracle
* Banco de dados IBM DB2
* Banco de dados IBM Informix (Beta)
* IBM Netezza
* Banco de dados MySQL
* Banco de dados PostgreSQL
* Banco de dados Sybase
* Banco de dados Teradata
* Banco de dados do SAP HANA
* Servidor de Aplicativos SAP Business Warehouse
* Servidor de Mensagens SAP Business Warehouse
* Amazon Redshift
* Impala
* Google BigQuery
* Vertica
* Snowflake
* Essbase
* Cubos do AtScale (Beta)
* Conector do BI
* Dremio
* Exasol
* Indexima (Beta)
* InterSystems IRIS (Beta)
* Jethro (Beta)
* Kyligence Enterprise (Beta)
* MarkLogic (Beta)

> [!NOTE]
> Alguns conectores de banco de dados exigem que você os habilite selecionando **Arquivo > Opções e configurações > Opções**, em seguida, **Recursos de Visualização** e habilitando o conector. Se você não vir alguns dos conectores mencionados acima e quiser usá-los, verifique suas configurações de **Recursos de Visualização**. Observe também que toda fonte de dados marcada como *Beta* ou *Visualização* tem suporte e funcionalidade limitados e não deve ser usada em ambientes de produção.

A imagem a seguir mostra a janela **Obter Dados** para **Banco de dados**.

![Obter Dados > Bancos de Dados](media/desktop-data-sources/data-sources_04.png)

A categoria **Power BI** fornece as seguintes conexões de dados:

* Conjuntos de dados do Power BI
* Fluxos de dados do Power BI

A imagem a seguir mostra a janela **Obter Dados** do **Power BI**.

![Obter Dados > Power BI](media/desktop-data-sources/data-sources_05.png)

A categoria **Azure** fornece as seguintes conexões de dados:

* Banco de dados SQL do Azure
* SQL Data Warehouse do Azure
* Banco de Dados do Azure Analysis Services
* Armazenamento de Blobs do Azure
* Armazenamento de Tabelas do Azure
* Azure Cosmos DB (Beta)
* Azure Data Lake Storage Gen1
* Azure HDInsight (HDFS)
* Azure HDInsight Spark
* Consulta Interativa do HDInsight
* Azure Data Explorer (Kusto)
* Gerenciamento de Custos do Azure (Beta)

A imagem a seguir mostra a janela **Obter Dados** para **Azure**.

![Obter Dados > Azure](media/desktop-data-sources/data-sources_06.png)

A categoria **Serviços Online** fornece as seguintes conexões de dados:

* Lista do SharePoint Online
* Microsoft Exchange Online
* Dynamics 365 (online)
* Dynamics NAV
* Dynamics 365 Business Central
* Central do Microsoft Dynamics 365 Business (local)
* Common Data Service
* Microsoft Azure Consumption Insights (Beta)
* Azure DevOps (Beta)
* Azure DevOps Server (Beta)
* Objetos do Salesforce
* Relatórios do Salesforce
* Google Analytics
* Adobe Analytics
* appFigures (Beta)
* Data.World – Obter Conjunto de Dados (Beta)
* Facebook
* GitHub (Beta)
* MailChimp (Beta)
* Merketo (Beta)
* Mixpanel (Beta)
* Planview Enterprise One – PRM (Beta)
* Planview Projectplace (Beta)
* QuickBooks Online (Beta)
* Smartsheet
* SparkPost (Beta)
* Stripe (Beta)
* SweetIQ (Beta)
* Planview Enterprise One – CMT (Beta)
* Twilio (Beta)
* tyGraph (Beta)
* Webtrends (Beta)
* ZenDesk (Beta)
* Fonte de dados do Emigo (Beta)
* Entersoft Business Suite (Beta)
* Industrial App Store
* Intune Data Warehouse (Beta)
* Segurança do Microsoft Graph (Beta)
* Quick Base
* TeamDesk (Beta)

A imagem a seguir mostra a janela **Obter Dados** para **Online Services**.

![Obter Dados > Serviços Online](media/desktop-data-sources/data-sources_07.png)

A categoria **Outros** fornece as seguintes conexões de dados:

* Web
* Lista do SharePoint
* Feed OData
* Active Directory
* Microsoft Exchange
* HDFS (Arquivo do Hadoop)
* Spark
* Script do R
* Script Python
* ODBC
* OLE DB
* BI360 – Relatórios Financeiros e Orçamento (Beta)
* Denado
* Grade de Informações (Beta)
* Paxata 
* QubolePresto (Beta)
* Roamler (Beta)
* SurveyMonkey (Beta)
* Tenforce (Smart)List (Beta)
* Workforce Dimensions (Beta)
* Consulta em Branco

A imagem a seguir mostra a janela **Obter Dados** para **Outros**.

![Obter Dados > Outros](media/desktop-data-sources/data-sources_08.png)

> [!NOTE]
> Neste momento, não é possível se conectar a fontes de dados personalizadas protegidas usando o Azure Active Directory.

## <a name="connecting-to-a-data-source"></a>Conectando a uma Fonte de Dados
Para se conectar a uma fonte de dados, selecione a fonte de dados na janela **Obter Dados** e selecione **Conectar**. Na imagem a seguir, a opção **Web** é selecionada na categoria de conexão de dados **Outros** .

![Conecte-se à Web](media/desktop-data-sources/data-sources_08.png)

É exibida uma janela de conexão específica para o tipo de conexão de dados usado. Se as credenciais forem necessárias, será solicitado que você as forneça. A imagem a seguir mostra uma URL sendo inserida para conectar a uma fonte de dados da Web.

![URL da Web de entrada](media/desktop-data-sources/datasources_fromwebbox.png)

Quando a URL ou as informações de conexão de recurso forem inseridas, selecione **OK**. O Power BI Desktop estabelece a conexão à fonte de dados e apresenta as fontes de dados disponíveis no **Navegador**.

![Tela do navegador](media/desktop-data-sources/datasources_fromnavigatordialog.png)

Você pode carregar os dados selecionando o botão **Carregar** na parte inferior do painel **Navegador** , ou editar a consulta antes de carregar dados selecionando o botão **Editar Consulta** .

Isso é tudo que é necessário para conectar a fontes de dados no Power BI Desktop. Tente se conectar aos dados da nossa crescente lista de fontes de dados e volte com frequência – continuamos aumentando à lista o tempo todo.

## <a name="next-steps"></a>Próximas etapas
Há inúmeras coisas que você pode fazer com o Power BI Desktop. Para obter mais informações sobre seus recursos, consulte as seguintes fontes:

* [O que é o Power BI Desktop?](desktop-what-is-desktop.md)
* [Visão geral de Consulta com o Power BI Desktop](desktop-query-overview.md)
* [Tipos de dados no Power BI Desktop](desktop-data-types.md)
* [Formatar e combinar dados com o Power BI Desktop](desktop-shape-and-combine-data.md)
* [Tarefas comuns de consulta no Power BI Desktop](desktop-common-query-tasks.md)    
