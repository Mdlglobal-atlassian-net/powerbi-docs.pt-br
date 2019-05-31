---
title: Solucionar Problemas ao iniciar o Power BI Desktop
description: Solucionar Problemas ao iniciar o Power BI Desktop
author: davidiseminger
manager: kfile
ms.reviewer: ''
ms.service: powerbi
ms.subservice: powerbi-desktop
ms.topic: conceptual
ms.date: 05/08/2019
ms.author: davidi
LocalizationGroup: Troubleshooting
ms.openlocfilehash: 19dc98b4f402176b2ae511236015ea25d7e4178b
ms.sourcegitcommit: 60dad5aa0d85db790553e537bf8ac34ee3289ba3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/29/2019
ms.locfileid: "65454421"
---
# <a name="resolve-issues-when-power-bi-desktop-will-not-launch"></a>Solucionar Problemas quando o Power BI Desktop não é iniciado
No **Power BI Desktop**, os usuários que instalaram e estão executando versões anteriores do **Gateway de dados local do Power BI** podem ser impedidos de iniciar o Power BI Desktop, devido às restrições de políticas administrativas que o gateway local do Power BI estabeleceu nos pipes nomeados no computador local. 

## <a name="resolve-issues-with-the-on-premises-data-gateway-and-power-bi-desktop"></a>Resolver problemas com o Gateway de dados local e o Power BI Desktop
Há três opções para resolver o problema associado ao Gateway de dados local e habilitar o Power BI Desktop para inicialização:

### <a name="resolution-1-install-the-latest-version-of-power-bi-on-premises-data-gateway"></a>Resolução 1: instalar a versão mais recente do Gateway de dados local do Power BI
A versão mais recente do Gateway de dados local do Power BI não coloca restrições de pipe nomeado no computador local e permite que o Power BI Desktop seja iniciado corretamente. Se você precisa continuar usando o Gateway de dados local do Power BI, esta é a resolução recomendada. Baixe a versão mais recente do Gateway de dados local do Power BI [neste local](https://go.microsoft.com/fwlink/?LinkId=698863). Observe que o link é um link de download direto para o executável da instalação.

### <a name="resolution-2-uninstall-or-stop-the-power-bi-on-premises-data-gateway-windows-service"></a>Resolução 2: desinstalar ou interromper o serviço Windows do Gateway de dados local do Power BI
Se você não precisa mais do Gateway de dados local do Power BI, é possível desinstalá-lo ou interromper o serviço Windows do Gateway de dados local do Power BI, que remove a restrição de política e permite que o Power BI Desktop seja iniciado.

### <a name="resolution-3-run-power-bi-desktop-with-administrator-privilege"></a>Resolução 3: executar o Power BI Desktop com privilégios de administrador
Como alternativa, você pode iniciar com êxito Power BI Desktop como administrador, que também permite que o Power BI Desktop seja iniciado com êxito. Ainda é recomendável que você instale a versão mais recente do Gateway de dados local do Power BI, conforme descrito anteriormente neste artigo.

É importante observar que o Power BI Desktop foi projetado como uma arquitetura multiprocesso, e vários desses processos se comunicam usando pipes nomeados do Windows. Pode haver outros processos que interferem com esses pipes nomeados. O motivo mais comum para essa interferência é a segurança, incluindo situações nas quais o software antivírus ou firewalls podem estar bloqueando os pipes ou redirecionando o tráfego para uma porta específica. Iniciar o Power BI Desktop com privilégios de administrador pode resolver esse problema. Se não for possível iniciá-lo com privilégios de administrador, entre em contato com o administrador para determinar quais regras de segurança estão sendo aplicadas que impedem a comunicação adequada dos pipes nomeados e inclua o Power BI Desktop e seus respectivos subprocessos na lista de permissões.

## <a name="resolve-issues-when-connecting-to-sql-server"></a>Solucionar problemas ao conectar-se ao SQL Server
Quanto você encontra uma mensagem de erro semelhante à seguinte ao se conectar a um banco de dados do SQL Server, geralmente é possível resolver o problema abrindo o **Power BI Desktop** como um administrador e, em seguida, fazendo a conexão com o SQL Server:

    "An error happened while reading data from the provider: 'Could not load file or assembly 'System.EnterpriseServices, Version=4.0.0.0, Culture=neutral, PublicKeyToken=xxxxxxxxxxxxx' or one of its dependencies. Either a required impersonation level was not provided, or the provided impersonation level is invalid. (Exception from HRESULT: 0x80070542)'"

Depois de iniciar como um administrador e estabelecer a conexão, as DLLs necessárias serão registradas corretamente. Depois disso, não será mais necessário iniciar o Power BI Desktop como um administrador.

## <a name="help-with-other-issues-when-launching-power-bi-desktop"></a>Ajuda com outros problemas ao iniciar o Power BI Desktop
Nos esforçamos para abordar o máximo possível de problemas que ocorrem com o **Power BI Desktop**. Examinamos regularmente os problemas que podem estar afetando muitos clientes, posteriormente incluindo-os em nossos artigos.

Se o problema ao iniciar o **Power BI Desktop** não estiver associado ao gateway de dados local ou se as resoluções anteriores não funcionarem, envie um incidente de suporte para o [suporte do Power BI](https://support.powerbi.com), https://support.powerbi.com) para ajudar você a identificar e resolver o problema.

Para outros problemas que você pode encontrar no futuro com o **Power BI Desktop** (esperamos que não ocorra nenhum ou que sejam poucos), é útil ativar o rastreamento e coletar arquivos de log, para melhor isolar e identificar o problema. Para ativar o rastreamento, selecione **Arquivo > Opções e configurações > Opções** e, em seguida, selecione **Diagnóstico**, depois, marque **Habilitar o rastreamento** em *Opções de diagnóstico*. Estamos cientes de que o **Power BI Desktop** deve estar em execução para que essa opção seja configurada, o que é mais útil para futuros problemas associados à inicialização do **Power BI Desktop**.

