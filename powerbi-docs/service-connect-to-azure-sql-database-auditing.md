---
title: Pacote de conteúdo de Auditoria de Banco de Dados SQL
description: Pacote de conteúdo de Auditoria de Banco de Dados SQL para o Power BI
author: SarinaJoan
manager: kfile
ms.reviewer: ''
ms.service: powerbi
ms.subservice: powerbi-template-apps
ms.topic: conceptual
ms.date: 11/09/2018
ms.author: sarinas
LocalizationGroup: Connect to services
ms.openlocfilehash: 0d212510fd2856fd509077f35e0f10bb7c5dd4c5
ms.sourcegitcommit: 60dad5aa0d85db790553e537bf8ac34ee3289ba3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/29/2019
ms.locfileid: "61180914"
---
# <a name="sql-database-auditing-content-pack-for-power-bi"></a>Pacote de conteúdo de Auditoria de Banco de Dados SQL para o Power BI

> [!IMPORTANT]
> O pacote de conteúdo de Auditoria de Banco de Dados SQL foi preterido e não está mais disponível.
 
O pacote de conteúdo do Power BI para a [Auditoria do Banco de Dados SQL](/azure/sql-database/sql-database-auditing/) do Azure permite que você entenda a atividade de seu banco de dados e obtenha informações sobre as discrepâncias e anomalias que podem gerar preocupações comerciais ou suspeitas de violações de segurança. 

Conecte-se ao [pacote de conteúdo da Auditoria do Banco de Dados SQL](https://app.powerbi.com/getdata/services/sql-db-auditing) para o Power BI.

>[!NOTE]
>O pacote de conteúdo importa dados de todas as tabelas que contêm “AuditLogs” no nome e acrescenta tudo a uma tabela única de modelo de dados chamada “AuditLogs”. Os últimos 250 mil eventos serão incluídos e os dados serão atualizados diariamente.

## <a name="how-to-connect"></a>Como se conectar
1. Selecione **Obter Dados** na parte inferior do painel de navegação esquerdo.
   
   ![](media/service-connect-to-azure-sql-database-auditing/pbi_getdata.png) 
2. Na caixa Serviços, selecione Obter.
   
   ![](media/service-connect-to-azure-sql-database-auditing/pbi_getservices.png) 
3. Selecione **Auditoria do Banco de Dados SQL** \> **Obter**.
   
   ![](media/service-connect-to-azure-sql-database-auditing/sqldbaudit.png)
4. Na janela Conectar à Auditoria do Banco de Dados SQL:
   
   - Insira o nome da conta de Armazenamento de Tabelas do Azure ou a URL em que os logs são armazenados.
   
   - Insira o nome do SQL Server desejado. Digite “\*” para carregar os logs de auditoria para todos os servidores.
   
   - Insira o nome do banco de dados SQL desejado. Digite “\*” para carregar os logs de auditoria para todos os bancos de dados.
   
   - Insira o nome da tabela do Azure que contém os logs desejados. Digite “\*” para carregar os logs de auditoria de todas as tabelas que contêm “AuditLogs” no nome.
   
   >[!IMPORTANT]
   >Por questões de desempenho, é recomendável sempre especificar um nome de tabela explícita, mesmo que todos os logs de auditoria sejam armazenados em uma única tabela.
   
   - Insira a data de início dos logs de auditoria desejados. Digite “\*” para carregar os logs de auditoria sem um tempo limite inferior ou “1d” para carregar os logs de auditoria do último dia.
   
   - Insira a data de término dos logs de auditoria desejados. Digite “\*” para carregar os logs de auditoria sem um tempo limite superior.
   
   ![](media/service-connect-to-azure-sql-database-auditing/dbauditing_param.png)
5. Como método de autenticação, selecione **Chave**, insira uma **chave de conta** \> **Entrar**.
   
   ![](media/service-connect-to-azure-sql-database-auditing/pbi_sqlauditing3.png)
6. Depois que o Power BI importar os dados, você verá um novo painel, relatório e conjunto de dados no painel de navegação esquerdo. Novos itens são marcados com um asterisco amarelo \*.
   
   ![](media/service-connect-to-azure-sql-database-auditing/pbi_sqldbauditingnewdash.png)

**E agora?**

* Tente [fazer uma pergunta na caixa de P e R](consumer/end-user-q-and-a.md) na parte superior do dashboard
* [Altere os blocos](service-dashboard-edit-tile.md) no dashboard.
* [Selecione um bloco](consumer/end-user-tiles.md) para abrir o relatório subjacente.
* Enquanto seu conjunto de dados será agendado para ser atualizado diariamente, você pode alterar o agendamento de atualização ou tentar atualizá-lo sob demanda usando **Atualizar Agora**

## <a name="next-steps"></a>Próximas etapas
[Obter dados para o Power BI](service-get-data.md)
[O que é o Power BI?](power-bi-overview.md)
