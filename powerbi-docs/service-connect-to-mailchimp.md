---
title: Conectar-se ao MailChimp com o Power BI
description: MailChimp para o Power BI
author: SarinaJoan
manager: kfile
ms.reviewer: maggiesMSFT
ms.service: powerbi
ms.subservice: powerbi-template-apps
ms.topic: conceptual
ms.date: 10/16/2017
ms.author: sarinas
LocalizationGroup: Connect to services
ms.openlocfilehash: e4986227b408dfec7ac10a880ff6110aa2ad5b9a
ms.sourcegitcommit: 750f0bfab02af24c8c72e6e9bbdd876e4a7399de
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/04/2019
ms.locfileid: "54007653"
---
# <a name="connect-to-mailchimp-with-power-bi"></a>Conectar-se ao MailChimp com o Power BI
O pacote de conteúdo do Power BI extrai dados de sua conta do MailChimp e gera um painel, um conjunto de relatórios e um conjunto de dados para permitir que você explore seus dados. Use a análise dos [painéis do MailChimp](https://powerbi.microsoft.com/integrations/mailchimp) para identificar rapidamente as tendências existentes em suas campanhas, seus relatórios e seus assinantes individuais. Os dados são configurados para serem atualizados diariamente, garantindo que os dados que você está monitorando são atuais.

Conecte-se ao [pacote de conteúdo do MailChimp](https://app.powerbi.com/getdata/services/mailchimp) para o Power BI.

## <a name="how-to-connect"></a>Como se conectar
1. Selecione **Obter Dados** na parte inferior do painel de navegação esquerdo.
   
    ![](media/service-connect-to-mailchimp/pbi_getdata.png)
2. Na caixa **Serviços** , selecione **Obter**.
   
   ![](media/service-connect-to-mailchimp/pbi_getservices.png)
3. Selecione **MailChimp** \> **Obter**.
   
   ![](media/service-connect-to-mailchimp/mailchimp.png)
4. Para o Método de Autenticação, selecione **oAuth2** \> **Entrar**.
   
    Quando solicitado, insira suas credenciais do MailChimp e siga o processo de autenticação.
   
    Na primeira vez que você se conectar, o Power BI solicitará a você o acesso somente leitura à sua conta. Selecione **Permitir** para iniciar o processo de importação, que pode levar alguns minutos dependendo do volume de dados em sua conta.
   
    ![](media/service-connect-to-mailchimp/allow.png)
5. Após o Power BI importar os dados, você verá novos elementos (painel, relatório e conjunto de dados) no painel de navegação esquerdo. Esse é o painel padrão criado pelo Power BI para exibir seus dados. Você pode alterar esse painel para exibir seus dados de qualquer modo que desejar.
   
   ![](media/service-connect-to-mailchimp/pbi_mailchimpnewdash.png)

**E agora?**

* Tente [fazer uma pergunta na caixa de P e R](consumer/end-user-q-and-a.md) na parte superior do dashboard
* [Altere os blocos](service-dashboard-edit-tile.md) no dashboard.
* [Selecione um bloco](consumer/end-user-tiles.md) para abrir o relatório subjacente.
* Enquanto seu conjunto de dados será agendado para ser atualizado diariamente, você pode alterar o agendamento de atualização ou tentar atualizá-lo sob demanda usando **Atualizar Agora**

## <a name="next-steps"></a>Próximas etapas
[O que é o Power BI?](power-bi-overview.md)

[Power BI – conceitos básicos](consumer/end-user-basic-concepts.md)

