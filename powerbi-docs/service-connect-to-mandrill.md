---
title: Conectar-se ao Mandrill com o Power BI
description: Mandrill para o Power BI
author: SarinaJoan
manager: kfile
ms.reviewer: maggiesMSFT
ms.service: powerbi
ms.subservice: powerbi-template-apps
ms.topic: conceptual
ms.date: 10/16/2017
ms.author: sarinas
LocalizationGroup: Connect to services
ms.openlocfilehash: efea81ab0a65b336e01c7a69af2189e31ae5d9f8
ms.sourcegitcommit: 762857c8ca09ce222cc3f8b006fa1b65d11e4ace
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/05/2019
ms.locfileid: "66721176"
---
# <a name="connect-to-mandrill-with-power-bi"></a>Conectar-se ao Mandrill com o Power BI
O pacote de conteúdo do Power BI extrai dados de sua conta do Mandrill e gera um painel, um conjunto de relatórios e um conjunto de dados para permitir que você explore seus dados. Use a análise do Mandrill para obter informações rapidamente sobre sua campanha de boletim informativo e de marketing. Os dados são configurados para serem atualizados diariamente, garantindo que os dados que você está monitorando são atuais.

Conecte-se ao [pacote de conteúdo do Mandrill para o Power BI.](http://app.powerbi.com/getdata/services/mandrill)

## <a name="how-to-connect"></a>Como se conectar
1. Selecione **Obter Dados** na parte inferior do painel de navegação esquerdo.
   
    ![](media/service-connect-to-mandrill/getdata.png)
2. Na caixa **Serviços** , selecione **Obter**.
   
    ![](media/service-connect-to-mandrill/services.png)
3. Selecione **Mandrill** > **Obter**.
   
    ![](media/service-connect-to-mandrill/mandrill.png)
4. Como o **Método de Autenticação**, selecione **Chave** e forneça sua chave de API. Você pode encontrar a chave na guia **Configurações** no painel do Mandrill. Selecione **Entrar** para iniciar o processo de importação, que pode levar alguns minutos dependendo do volume de dados em sua conta.
   
    ![](media/service-connect-to-mandrill/auth.png)
5. Após o Power BI importar os dados, você verá novos elementos (painel, relatório e conjunto de dados) no painel de navegação esquerdo. Esse é o painel padrão criado pelo Power BI para exibir seus dados.
   
    ![](media/service-connect-to-mandrill/mandrill-dashboard1.jpg)

**E agora?**

* Tente [fazer uma pergunta na caixa de P e R](consumer/end-user-q-and-a.md) na parte superior do dashboard
* [Altere os blocos](service-dashboard-edit-tile.md) no dashboard.
* [Selecione um bloco](consumer/end-user-tiles.md) para abrir o relatório subjacente.
* Enquanto seu conjunto de dados será agendado para ser atualizado diariamente, você pode alterar o agendamento de atualização ou tentar atualizá-lo sob demanda usando **Atualizar Agora**

## <a name="next-steps"></a>Próximas etapas
[O que é o Power BI?](power-bi-overview.md)

[Conceitos básicos para designers no serviço do Power BI](service-basic-concepts.md)

