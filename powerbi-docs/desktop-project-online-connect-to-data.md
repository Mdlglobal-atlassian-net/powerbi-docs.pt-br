---
title: 'Project Online: conectar-se aos dados por meio do Power BI Desktop'
description: 'Project Online: conectar-se aos dados por meio do Power BI Desktop'
author: davidiseminger
manager: kfile
ms.reviewer: ''
ms.service: powerbi
ms.component: powerbi-desktop
ms.topic: conceptual
ms.date: 11/28/2018
ms.author: davidi
LocalizationGroup: Connect to data
ms.openlocfilehash: 3773f1cb13eb967c511245f57cf59c7159d68fba
ms.sourcegitcommit: 2ae660a7b70fce23eb58b159d049eca44a664f2c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2018
ms.locfileid: "52669878"
---
# <a name="project-online-connect-to-data-through-power-bi-desktop"></a>Project Online: conectar-se aos dados por meio do Power BI Desktop
Você pode conectar-se a dados no Project Online por meio do Power BI Desktop.

### <a name="step-1-download-power-bi-desktop"></a>Etapa 1: Baixar o Power BI Desktop
1. [Baixar o Power BI Desktop](http://go.microsoft.com/fwlink/?LinkID=521662) e, em seguida, execute o instalador para obter o **Power BI Desktop** em seu computador.

### <a name="step-2-connect-to-project-online-with-odata"></a>Etapa 2: Conectar-se ao Project Online com o OData
1. Abra o **Power BI Desktop**.
2. Na tela de *Boas-vindas*, selecione **Obter dados**.
3. Escolha **feed OData** e selecione **Conectar**.
4. Insira o endereço para o feed OData na caixa URL e, em seguida, clique em OK.
   
   Se o endereço do seu site do Project Web App for semelhante a https://\<nomedolocatário\>.sharepoint.com/sites/pwa, o endereço que você inserirá para o Feed OData será https://\<nomedolocatário\>.sharepoint.com/sites/pwa/\_api/Projectdata.
   
   Para nosso exemplo, estamos usando https://contoso.sharepoint.com/sites/pwa/default.aspx
5. O Power BI Desktop solicitará que você se autentique com sua conta do Office 365. Selecione Conta organizacional e, em seguida, insira suas credenciais.
   
   ![](media/desktop-project-online-connect-to-data/image.png)

Observe que a conta usada para se conectar ao feed OData deve ter pelo menos o acesso pelo Visualizador de Portfólio ao site do aplicativo Web do projeto. 

Aqui, você pode escolher a quais tabelas deseja se conectar e criar uma consulta.  Quer uma ideia de como começar?  A postagem de blog a seguir mostra como criar um gráfico de burndown com base em seus dados do Project Online.  A postagem de blog refere-se ao uso do Power Query para se conectar ao Project Online, mas isso se aplica também ao Power BI Desktop.

[Criação de gráficos de burndown para o Project usando o Power Pivot e o Power Query](http://blogs.office.com/2014/03/24/creating-burndown-charts-for-project-using-power-pivot-and-power-query/)

