---
title: URLs do Power BI
description: Este artigo descreve os pontos de extremidade que devem ser acessíveis para clientes que usam o Power BI.
author: mgblythe
ms.author: mblythe
manager: kfile
ms.reviewer: ''
ms.service: powerbi
ms.component: powerbi-service
ms.topic: conceptual
ms.date: 10/22/2018
ms.openlocfilehash: cc7b24d273f8e83854f7e316f0c761e710e48160
ms.sourcegitcommit: a764e4b9d06b50d9b6173d0fbb7555e3babe6351
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2018
ms.locfileid: "49641955"
---
# <a name="power-bi-urls"></a>URLs do Power BI

**O serviço online do Power BI**, também conhecido como aplicativo SaaS (Software como serviço) do Power BI, requer conectividade com a Internet. Os pontos de extremidade abaixo devem ser acessíveis para clientes que usam o serviço online do Power BI.

Para usar o serviço online do Power BI, é necessário ter acesso para se conectar aos pontos de extremidade marcados como **necessários** nas tabelas abaixo e quaisquer pontos de extremidade marcados como **necessários** nos sites vinculados. Se o link para um site externo se referir a uma seção específica, será necessário apenas analisar os pontos de extremidade nessa seção.

Os pontos de extremidade marcados como **opcionais** também podem ser adicionados à **lista de permissões** para uma funcionalidade específica funcionar.

O serviço online do Power BI requer apenas que a porta TCP 443 seja aberta para os pontos de extremidade listados.

Caracteres curinga (*) representam todos os níveis sob o domínio raiz, e usaremos N/D quando as informações não estiverem disponíveis. A coluna **Destino(s)** é uma lista com domínios/FQDN e links para sites externos, que contêm mais informações sobre o ponto de extremidade.

>[!Important]
>As informações nas tabelas abaixo não representam a **nuvem do Governo dos EUA**, **a nuvem da Alemanha** ou a **nuvem da China**.

## <a name="authentication"></a>Autenticação

O Power BI depende dos pontos de extremidade necessários nas seções de identidade e autenticação do Office 365. Para usar o Power BI, conecte-se aos pontos de extremidade no site vinculado abaixo.

| Linha | Finalidade | Destino(s) | Porta(s) |
| --- | --- | --- | --- |
| 1 | **Obrigatório:** autenticação e identidade | Confira a documentação do Office 365 do [Office Online e URLs comuns](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges#microsoft-365-common-and-office-online)  | N/A |

## <a name="general-site-usage"></a>Uso geral do site

Para o uso geral do Power BI, conecte-se aos pontos de extremidade na tabela e nos sites vinculados abaixo.

| Linha | Finalidade | Destino(s) | Porta(s) |
| --- | --- | --- | --- |
| 1 | **Obrigatório:** APIs de back-end | *.analysis.windows.net | TCP 443 |
| 2 | **Obrigatório:** integração do Office 365 | Confira a documentação do Office 365 do [Office Online e URLs comuns](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges#microsoft-365-common-and-office-online) | N/A |
| 3 | **Obrigatório:** Portal | app.powerbi.com | TCP 443 |
| 4 | **Obrigatório:** telemetria de serviço | dc.services.visualstudio.com | TCP 443 |
| 5 | **Opcional:** mensagens informativas | dynmsg.modpim.com | TCP 443 |
| 6 | **Opcional:** pesquisas NPS | nps.onyx.azure.net | TCP 443 |
| | | |

## <a name="administration"></a>Administração

Para executar funções administrativas dentro do Power BI, conecte-se aos pontos de extremidade nos sites vinculados abaixo.

| Linha | Finalidade | Destino(s) | Porta(s) |
| --- | --- | --- | --- |
| 1 | **Obrigatório:** para gerenciar usuários e exibir logs de auditoria | Confira a documentação do Office 365 do [Office Online e URLs comuns](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges#microsoft-365-common-and-office-online) | N/A |
| | | |

## <a name="getting-data"></a>Obtendo dados

Para obter dados de fontes de dados específicas, como o OneDrive, você deve ser capaz de se conectar aos pontos de extremidade na tabela abaixo. O acesso a URLs e domínios de Internet adicionais pode ser necessário para fontes de dados específicas usadas dentro da sua organização.

| Linha | Finalidade | Destino(s) | Porta(s) |
| --- | --- | --- | --- |
| 1 | **Obrigatório:** AppSource (aplicativos internos ou externos no Power BI) | appsource.microsoft.com </br> *.s-microsoft.com  | TCP 443 |
| 2 | **Obrigatório:** entrar e obter dados para os pacotes de conteúdo | *.github.com  | TCP 443 |
| 3 | **Opcional:** importar arquivos do OneDrive pessoal | Consulte o site [URLs e portas necessárias para o OneDrive](https://docs.microsoft.com/en-us/onedrive/required-urls-and-ports) | N/A |
| 4 | **Opcional:** vídeo de tutorial do Power BI em 60 segundos | *.doubleclick.net </br> *.ggpht.com </br> *.google.com </br> *.googlevideo.com </br> *.youtube.com </br> *.ytimg.com </br> fonts.gstatic.com | TCP 443 |
| 5 | **Opcional:** fontes de dados de streaming do PubNub | Consulte a [documentação do PubNub](https://support.pubnub.com/support/solutions/articles/14000043522) | N/A |
| | | |

## <a name="dashboard-and-report-integration"></a>Integração do dashboard e do relatório

O Power BI depende de determinados pontos de extremidade para poder dar suporte aos seus dashboards e relatórios. Você deve poder se conectar aos pontos de extremidade na tabela e nos sites vinculados abaixo.

| Linha | Finalidade | Destino(s) | Porta(s) |
| --- | --- | --- | --- |
| 1 | **Obrigatório:** integração do Excel | Confira a documentação do Office 365 do [Office Online e URLs comuns](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges#microsoft-365-common-and-office-online) | N/A |
| | | |

## <a name="custom-visuals"></a>Visuais personalizados

O Power BI depende de determinados pontos de extremidade para poder exibir e acessar os visuais personalizados. Você deve poder se conectar aos pontos de extremidade na tabela e nos sites vinculados abaixo.

| Linha | Finalidade | Destino(s) | Porta(s) |
| --- | --- | --- | --- |
| 1 | **Obrigatório:** importar um visual personalizado da interface do Marketplace ou de um arquivo | *.azureedge.net </br> *.blob.core.windows.net </br> store.office.com | TCP 443 |
| 2 | **Opcional:** Bing Mapas | bing.com </br> platform.bing.com </br> *.dynamic.tiles.virtualearth.net </br> *.virtualearth.net | TCP 443 |
| 3 | **Opcional:** PowerApps | Consulte a [seção Serviços necessários](https://docs.microsoft.com/powerapps/maker/canvas-apps/limits-and-config#required-services) no site de requisitos de sistema do PowerApps | N/A |
| 4 | **Opcional:** Visio | Confira a documentação do Office 365 para [Office Online e URLs comuns](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges#microsoft-365-common-and-office-online), bem como [SharePoint Online e OneDrive for Business](https://docs.microsoft.com/en-us/office365/enterprise/urls-and-ip-address-ranges#sharepoint-online-and-onedrive-for-business) | N/A |
| | | |

## <a name="related-external-sites"></a>Sites externos relacionados

O Power BI contém links para outros sites relacionados. Esses sites incluem os de documentação, suporte, solicitações de novos recursos e muito mais. Esses sites não afetarão a funcionalidade do Power BI, portanto podem ser opcionalmente incluídos na lista de permissões se desejado.

| Linha | Finalidade | Destino(s) | Porta(s) |
| --- | --- | --- | --- |
| 1 | **Opcional:** site da comunidade | community.powerbi.com </br> oxcrx34285.i.lithium.com | TCP 443 |
| 2 | **Opcional:** site da documentação | docs.microsoft.com </br> img-prod-cms-rt-microsoft-com.akamaized.net </br> statics-uhf-eas.akamaized.net </br> cdnssl.clicktale.neting-district.clicktale.net | TCP 443 |
| 3 | **Opcional:** site de Download (para o Power BI Desktop etc.) | download.microsoft.com | TCP 443 |
| 4 | **Opcional:** redirecionamentos externos | aka.ms </br> go.microsoft.com | TCP 443 |
| 5 | **Opcional:** site de feedback de ideias| ideas.powerbi.com </br> powerbi.uservoice.com | TCP 443 |
| 6 | **Opcional:** site do Power BI – página de aterrissagem, links para saber mais, site de suporte, links de download, demonstração do parceiro etc. | powerbi.microsoft.com | TCP 443 |
| 7 | **Opcional:** Central de Desenvolvedores do Power BI | dev.powerbi.com | TCP 443 |
| 8 | **Opcional:** Site de suporte | support.powerbi.com </br> s3.amazonaws.com </br> *.olark.com </br> logx.optimizely.com </br> mscom.demdex.net </br> tags.tiqcdn.com | TCP 443 |
| | | |