---
title: Solucionando problemas da atualização agendada para Bancos de Dados SQL do Azure
description: Solucionando problemas em atualização agendada para bancos de dados SQL Azure no Power BI
author: maggiesMSFT
ms.reviewer: kayu
ms.service: powerbi
ms.subservice: powerbi-service
ms.topic: troubleshooting
ms.date: 09/04/2019
ms.author: maggies
ms.custom: seodec18
LocalizationGroup: Troubleshooting
ms.openlocfilehash: 292f80b4fec7da9ff6ce42e3611bf4d6353bae2d
ms.sourcegitcommit: 0e9e211082eca7fd939803e0cd9c6b114af2f90a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "83280462"
---
# <a name="troubleshooting-scheduled-refresh-for-azure-sql-databases-in-power-bi"></a>Solucionando problemas em atualização agendada para bancos de dados SQL Azure no Power BI

Para informações detalhadas sobre a atualização, confira [Atualizar dados no Power BI](refresh-data.md) e [Configurar atualização programada](refresh-scheduled-refresh.md).

Ao configurar a atualização agendada para o Banco de Dados SQL do Azure, se você receber um erro com o código de erro 400 durante a edição de credenciais, tente o seguinte para configurar a regra de firewall apropriada:

1. Conecte-se com o [Portal do Azure](https://portal.azure.com).

1. Acesse o Banco de Dados SQL do Azure para o qual você está configurando a atualização.

1. Na parte superior da folha **Visão Geral**, selecione **Definir firewall do servidor**.

1. Na folha **Configurações de firewall**, verifique se **Permitir o acesso aos serviços do Azure** está definido como **LIGADO**.

    ![Serviços permitidos do Azure](media/service-admin-troubleshooting-scheduled-refresh-azure-sql-databases/azurerefresh.png)  

Mais perguntas? [Experimente a Comunidade do Power BI](https://community.powerbi.com/)
