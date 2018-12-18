---
title: Capturando de informações adicionais de diagnóstico
description: Capturando de informações adicionais de diagnóstico
author: mgblythe
manager: kfile
ms.reviewer: ''
ms.service: powerbi
ms.component: powerbi-service
ms.topic: conceptual
ms.date: 06/28/2017
ms.author: mblythe
ms.custom: seodec18
LocalizationGroup: Troubleshooting
ms.openlocfilehash: 8a8ec433a6ebb620593648cdb222df0f60b2f21e
ms.sourcegitcommit: 72c9d9ec26e17e94fccb9c5a24301028cebcdeb5
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2018
ms.locfileid: "53025125"
---
# <a name="capturing-additional-diagnostic-information"></a>Capturando de informações adicionais de diagnóstico
## <a name="capturing-additional-diagnostic-information-for-power-bi"></a>Capturar Informações de Diagnóstico Adicionais para o Power BI
Estas instruções fornecem duas opções possíveis para coletar manualmente as informações adicionais de diagnóstico do cliente Web Power BI.  Somente uma dessas opções deve ser seguida.

## <a name="network-capture---edge--internet-explorer"></a>Captura de rede – Edge e Internet Explorer
1. Navegue até [Power BI](https://app.powerbi.com) com o Microsoft Edge ou Internet Explorer.
2. Abra as ferramentas de desenvolvedor do Edge pressionando F12.
3. Isso abrirá a janela de Ferramentas de Desenvolvedor: 
   
   ![Ferramentas de desenvolvedor](media/service-admin-capturing-additional-diagnostic-information-for-power-bi/edge-developer-tools.png)
4. Mude para a guia Rede. Ele listará o tráfego que já foi capturado. 
   
   ![Guia de rede do Edge](media/service-admin-capturing-additional-diagnostic-information-for-power-bi/edge-network-tab.png)
5. É possível navegar na janela e reproduzir qualquer problema que talvez você esteja enfrentando. Você pode ocultar e mostrar a janela de ferramentas de desenvolvedor a qualquer momento durante a sessão, pressionando F12.
6. Para interromper a captura, é possível selecionar o quadrado vermelho na guia Rede da área de ferramentas de desenvolvedor.
   
   ![Interromper a captura](media/service-admin-capturing-additional-diagnostic-information-for-power-bi/edge-network-tab-stop.png)
7. Selecione o ícone de disquete para **Exportar como HAR**
   
   ![Exportar o arquivo](media/service-admin-capturing-additional-diagnostic-information-for-power-bi/edge-network-tab-save.png)
8. Forneça um nome de arquivo e salve o arquivo HAR.
   
    O arquivo HAR contém todas as informações sobre solicitações de rede entre a janela do navegador e o Power BI.  Isso incluirá as IDs de atividade para cada solicitação, o carimbo de data/hora preciso para cada solicitação e qualquer informação de erro retornado ao cliente.  Este rastreamento também conterá os dados usados para preencher os elementos visuais mostrados na tela.
9. Você pode fornecer o arquivo HAR para dar suporte à análise.

Mais perguntas? [Experimente perguntar à Comunidade do Power BI](http://community.powerbi.com/)

