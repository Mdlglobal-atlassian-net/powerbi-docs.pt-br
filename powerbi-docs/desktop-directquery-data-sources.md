---
title: Fontes de dados com suporte do DirectQuery no Power BI
description: Obtenha uma lista de quais fontes de dados podem usar o DirectQuery.
author: davidiseminger
ms.author: davidi
manager: kfile
ms.reviewer: ''
ms.service: powerbi
ms.subservice: powerbi-desktop
ms.topic: conceptual
ms.date: 11/01/2018
LocalizationGroup: Connect to data
ms.openlocfilehash: 84e40e9fbce07716a2250a58bfcbd396a40d2842
ms.sourcegitcommit: 796bf513bf8669676e2a44627b56221b1629a6a8
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "56826550"
---
# <a name="data-sources-supported-by-directquery-in-power-bi"></a>Fontes de dados com suporte do DirectQuery no Power BI

O **Power BI Desktop** e o **serviço do Power BI** têm várias fontes de dados às quais você pode se conectar para obter acesso aos dados. Este artigo descreve quais fontes de dados do Power BI dão suporte ao método de conexão conhecido como **DirectQuery**. Para obter mais informações sobre o DirectQuery, consulte [**DirectQuery no Power BI**](desktop-directquery-about.md).

As seguintes fontes de dados dão suporte ao DirectQuery no Power BI:

* Amazon Redshift
* Azure HDInsight Spark (Beta)
* Banco de dados SQL do Azure
* SQL Data Warehouse do Azure
* Google BigQuery (Beta)
* Banco de dados IBM DB2
* IBM Netezza (Beta)
* Impala (versão 2.x)
* Banco de Dados Oracle (versão 12 e posterior)
* Servidor de Aplicativos SAP Business Warehouse
* Servidor de Mensagens SAP Business Warehouse (Beta)
* SAP HANA
* Snowflake
* Spark (Beta) (versão 0.9 e posterior)
* SQL Server
* Banco de dados Teradata
* Vertica (Beta)

As fontes de dados que têm **(Beta)** ou **(Versão prévia)** depois do nome estão sujeitas a alterações e não há suporte para que elas sejam usadas em produção. É possível que também não haja suporte para elas após a publicação de um relatório no **serviço do Power BI**, o que significa que abrir um relatório publicado ou explorar o conjunto de dados pode resultar em um erro.

A única diferença entre fontes de dados **(Beta)** e em **(Versão prévia)** é que as fontes em **(Versão prévia)** precisam ser habilitadas como um recurso de versão prévia antes que fiquem disponíveis para uso. Para habilitar um conector de dados em **(Versão prévia)**, no **Power BI Desktop**, acesse **Arquivo > Opções e Configurações > Opções** e, em seguida, **Recursos de versão prévia**.

> [!NOTE]
> Consultas DirectQuery para SQL Server requerem autenticação usando as credenciais de autenticação atuais do Windows ou credenciais de banco de dados para estabelecer o acesso. Credenciais alternativas não são compatíveis.
>

## <a name="on-premises-gateway-requirements"></a>Requisitos de gateway local
A tabela a seguir especifica se um **Gateway de dados local** é necessário para se conectar à fonte de dados especificada após publicar um relatório no **serviço do Power BI**.

| Fonte | Gateway necessário? |
| --- | --- |
| SQL Server |Sim |
| Banco de dados SQL do Azure |Não |
| SQL Data Warehouse do Azure |Não |
| SAP HANA |Sim |
| Banco de dados Oracle |Sim |
| Banco de dados Teradata |Sim |
| Amazon Redshift |Não |
| Impala (versão 2.x) |Sim |
| Snowflake |Sim |
| Spark (beta), versão 0.9 e posterior |Sim |
| Azure HDInsight Spark (Beta) |Não |
| IBM Netezza |Sim |
| Servidor de Aplicativos SAP Business Warehouse |Sim |
| Servidor de Mensagens SAP Business Warehouse |Ainda não tem suporte no **serviço do Power BI** |
| Google BigQuery |Não |


## <a name="next-steps"></a>Próximas etapas
Para obter mais informações sobre o DirectQuery, confira os seguintes recursos:

* [DirectQuery no Power BI](desktop-directquery-about.md)
* [DirectQuery e SAP HANA](desktop-directquery-sap-hana.md)
* [DirectQuery e SAP BW](desktop-directquery-sap-bw.md)
* [Gateway de dados local](service-gateway-onprem.md)

