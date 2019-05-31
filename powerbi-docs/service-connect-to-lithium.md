---
title: Conectar-se ao Lithium com o Power BI
description: Lithium para o Power BI
author: SarinaJoan
manager: kfile
ms.reviewer: maggiesMSFT
ms.service: powerbi
ms.subservice: powerbi-template-apps
ms.topic: conceptual
ms.date: 10/16/2017
ms.author: sarinas
LocalizationGroup: Connect to services
ms.openlocfilehash: 9029d5b6268cacf17fc862a4c0a3d19f440f7de1
ms.sourcegitcommit: 60dad5aa0d85db790553e537bf8ac34ee3289ba3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/29/2019
ms.locfileid: "61163778"
---
# <a name="connect-to-lithium-with-power-bi"></a>Conectar-se ao Lithium com o Power BI
O Lithium cria relações de confiança entre marcas melhor do mundo e seus clientes, ajudando as pessoas a obter respostas e compartilhar suas experiências. Conectando o pacote de conteúdo do Lithium para o Power BI, você pode medir métricas-chave sobre sua comunidade online para ajudar a estimular as vendas, reduzir os custos de serviço e aumentar a fidelidade. 

Conecte-se ao [pacote de conteúdo do Lithium](https://app.powerbi.com/getdata/services/lithium) para o Power BI.

>[!NOTE]
>O pacote de conteúdo do Power BI usa a API do Lithium. Excesso chamadas para a API podem resultar em encargos adicionais do Lithium, confirme com seu administrador do Lithium.

## <a name="how-to-connect"></a>Como se conectar
1. Selecione **Obter Dados** na parte inferior do painel de navegação esquerdo.
   
   ![](media/service-connect-to-lithium/pbi_getdata.png) 
2. Na caixa **Serviços** , selecione **Obter**.
   
   ![](media/service-connect-to-lithium/pbi_getservices.png) 
3. Selecione **Lithium** \> **Obter**.
   
   ![](media/service-connect-to-lithium/lithiumconnect.png)
4. Forneça a URL de sua comunidade do Lithium. Ela estará no formato *https://community.yoursite.com* .
   
   ![](media/service-connect-to-lithium/params.png)
5. Quando solicitado, insira suas credenciais do Lithium. Selecione **oAuth 2** como o mecanismo de autenticação, clique em **Entrar** e siga o fluxo de autenticação do Lithium.
   
   ![](media/service-connect-to-lithium/creds.png)
   
   ![](media/service-connect-to-lithium/creds2.png)
6. Quando o fluxo de logon estiver concluído, o processo de importação será iniciado. Quando concluído, um novo painel, relatório e modelo aparecerão no Painel de Navegação. Selecione o painel para exibir os dados importados por você.
   
    ![](media/service-connect-to-lithium/lithium.png)

**E agora?**

* Tente [fazer uma pergunta na caixa de P e R](consumer/end-user-q-and-a.md) na parte superior do dashboard
* [Altere os blocos](service-dashboard-edit-tile.md) no dashboard.
* [Selecione um bloco](consumer/end-user-tiles.md) para abrir o relatório subjacente.
* Enquanto seu conjunto de dados será agendado para ser atualizado diariamente, você pode alterar o agendamento de atualização ou tentar atualizá-lo sob demanda usando **Atualizar Agora**

## <a name="system-requirements"></a>Requisitos de sistema
O pacote de conteúdo do Lithium exige uma comunidade do Lithium v15.9 ou superior. Entre em contato com seu administrador do Lithium para confirmar.

## <a name="next-steps"></a>Próximas etapas
[O que é o Power BI?](power-bi-overview.md)

[Power BI – conceitos básicos](consumer/end-user-basic-concepts.md)

