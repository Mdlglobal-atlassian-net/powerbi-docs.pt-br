---
title: Fontes de dados no Power BI Desktop
description: Fontes de dados no Power BI Desktop
services: powerbi
documentationcenter: 
author: davidiseminger
manager: kfile
backup: 
editor: 
tags: 
qualityfocus: complete
qualitydate: 04/29/2016
ms.service: powerbi
ms.devlang: NA
ms.topic: article
ms.tgt_pltfrm: NA
ms.workload: powerbi
ms.date: 10/05/2017
ms.author: davidi
ms.openlocfilehash: 6014b38e0e9cabe0dc909268f87cdb284de47106
ms.sourcegitcommit: 284b09d579d601e754a05fba2a4025723724f8eb
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/15/2017
---
# <a name="data-sources-in-power-bi-desktop"></a>Fontes de dados no Power BI Desktop
O Power BI Desktop permite se conectar a dados de várias fontes diferentes. Veja uma lista completa das fontes de dados disponíveis na parte inferior desta página.

Para se conectar a dados, selecione **Obter Dados** na faixa de opções **Página Inicial** . Selecionar a seta para baixo ou o texto **Obter Dados** no botão exibe o menu de tipos de dados **Mais Comuns** mostrado na imagem a seguir.

![](media/desktop-data-sources/data-sources_1.png)

Selecionar **Mais...** no menu **Mais Comuns** exibe a janela **Obter Dados**. Você também pode abrir a janela **Obter Dados** (e ignorar o menu **Mais Comuns** ) selecionando diretamente o **botão do ícone** **Obter Dados** .

![](media/desktop-data-sources/data-sources_2.png)

> [!NOTE]
> A equipe do Power BI está sempre expandindo as fontes de dados disponíveis para o **Power BI Desktop** e o **serviço do Power BI**. Assim, você verá com frequência as versões anteriores das fontes de dados de trabalho em andamento marcadas como *Beta* ou *Visualização*. Toda fonte de dados marcada como *Beta* ou *Visualização* tem suporte e funcionalidade limitados e não deve ser usada em ambientes de produção.
> 
> 

## <a name="data-sources"></a>Fontes de Dados
Tipos de dados são organizados nas categorias a seguir:

* Todos
* Arquivo
* Banco de dados
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
* Pasta do SharePoint

A imagem a seguir mostra a janela **Obter Dados** para **Arquivo**.

![](media/desktop-data-sources/data-sources_3.png)

> [!NOTE]
> Em versões anteriores do Power BI Desktop, **CSV** e **texto** eram tipos de conexão de dados separados. Esses conectores de dados foram combinados em **CSV/Texto**.
> 
> 

A categoria **Banco de dados** fornece as seguintes conexões de dados:

* Banco de dados do SQL Server
* Banco de dados do Access
* Banco de dados do SQL Server Analysis Services
* Banco de dados Oracle
* Banco de dados IBM DB2
* Banco de dados IBM Informix (Beta)
* IBM Netezza (Beta)
* Banco de dados MySQL
* Banco de dados PostgreSQL
* Banco de dados Sybase
* Banco de dados Teradata
* Banco de dados do SAP HANA
* Servidor do SAP Business Warehouse
* Amazon Redshift
* Impala
* Google BigQuery (Beta)
* Snowflake

> [!NOTE]
> Alguns conectores de banco de dados exigem que você os habilite selecionando **Arquivo > Opções e configurações > Opções**, em seguida, **Recursos de Visualização** e habilitando o conector. Se você não vir alguns dos conectores mencionados acima e quiser usá-los, verifique suas configurações de **Recursos de Visualização**. Observe também que toda fonte de dados marcada como *Beta* ou *Visualização* tem suporte e funcionalidade limitados e não deve ser usada em ambientes de produção.
> 
> 

A imagem a seguir mostra a janela **Obter Dados** para **Banco de dados**.

![](media/desktop-data-sources/data-sources_4.png)

A categoria **Azure** fornece as seguintes conexões de dados:

* Banco de dados SQL do Azure
* SQL Data Warehouse do Azure
* Banco de dados do Analysis Services do Azure (Beta)
* Armazenamento de Blobs do Azure
* Armazenamento de Tabelas do Azure
* Azure Cosmos DB (Beta)
* Azure Data Lake Store
* Azure HDInsight (HDFS)
* Azure HDInsight Spark (Beta)

A imagem a seguir mostra a janela **Obter Dados** para **Azure**.

![](media/desktop-data-sources/data-sources_5.png)

A categoria **Serviços Online** fornece as seguintes conexões de dados:

* Serviço do Power BI
* Lista do SharePoint Online
* Microsoft Exchange Online
* Dynamics 365 (online)
* Dynamics 365 for Financials (Beta)
* Common Data Service (Beta)
* Microsoft Azure Consumption Insights (Beta)
* Visual Studio Team Services (Beta)
* Objetos do Salesforce
* Relatórios do Salesforce
* Google Analytics
* appFigures (Beta)
* comScore Digital Analytix (Beta)
* Dynamics 365 para Customer Insights (Beta)
* Facebook
* GitHub (Beta)
* Kusto (Beta)
* MailChimp (Beta)
* Mixpanel (Beta)
* Planview Enterprise (Beta)
* Projectplace (Beta)
* QuickBooks Online (Beta)
* Smartsheet
* SparkPost (Beta)
* SQL Sentry (Beta)
* Stripe (Beta)
* SweetIQ (Beta)
* Troux (Beta)
* Twilio (Beta)
* tyGraph (Beta)
* Webtrends (Beta)
* ZenDesk (Beta)

A imagem a seguir mostra a janela **Obter Dados** para **Online Services**.

![](media/desktop-data-sources/data-sources_6b.png)

A categoria **Outros** fornece as seguintes conexões de dados:

* Vertica (Beta)
* Web
* Lista do SharePoint
* Feed OData
* Active Directory
* Microsoft Exchange
* HDFS (Arquivo do Hadoop)
* Spark (Beta)
* Script do R
* ODBC
* OLE DB
* Consulta em Branco

A imagem a seguir mostra a janela **Obter Dados** para **Outros**.

![](media/desktop-data-sources/data-sources_7a.png)

> [!NOTE]
> Neste momento, não é possível se conectar a fontes de dados personalizadas protegidas usando o Azure Active Directory.
> 
> 

## <a name="connecting-to-a-data-source"></a>Conectando a uma Fonte de Dados
Para se conectar a uma fonte de dados, selecione a fonte de dados na janela **Obter Dados** e selecione **Conectar**. Na imagem a seguir, a opção **Web** é selecionada na categoria de conexão de dados **Outros** .

![](media/desktop-data-sources/data-sources_7b.png)

É exibida uma janela de conexão específica para o tipo de conexão de dados usado. Se as credenciais forem necessárias, será solicitado que você as forneça. A imagem a seguir mostra uma URL sendo inserida para conectar a uma fonte de dados da Web.

![](media/desktop-data-sources/datasources_fromwebbox.png)

Quando a URL ou as informações de conexão de recurso forem inseridas, selecione **OK**. O Power BI Desktop estabelece a conexão à fonte de dados e apresenta as fontes de dados disponíveis no **Navegador**.

![](media/desktop-data-sources/datasources_fromnavigatordialog.png)

Você pode carregar os dados selecionando o botão **Carregar** na parte inferior do painel **Navegador** , ou editar a consulta antes de carregar dados selecionando o botão **Editar Consulta** .

Isso é tudo que é necessário para conectar a fontes de dados no Power BI Desktop. Tente se conectar aos dados da nossa crescente lista de fontes de dados e volte com frequência – continuamos aumentando à lista o tempo todo.

## <a name="next-steps"></a>Próximas etapas
Há inúmeras coisas que você pode fazer com o Power BI Desktop. Para obter mais informações sobre seus recursos, consulte as seguintes fontes:

* [Introdução ao Power BI Desktop](desktop-getting-started.md)
* [Visão geral de Consulta com o Power BI Desktop](desktop-query-overview.md)
* [Tipos de dados no Power BI Desktop](desktop-data-types.md)
* [Formatar e combinar dados com o Power BI Desktop](desktop-shape-and-combine-data.md)
* [Tarefas comuns de consulta no Power BI Desktop](desktop-common-query-tasks.md)    
