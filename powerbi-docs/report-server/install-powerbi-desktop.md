---
title: Instalar o Power BI Desktop otimizado para o Servidor de Relatório do Power BI
description: Saiba como instalar o Power BI Desktop otimizado para o Servidor de Relatório do Power BI
author: maggiesMSFT
manager: kfile
ms.reviewer: ''
ms.service: powerbi
ms.subservice: powerbi-report-server
ms.topic: conceptual
ms.date: 09/19/2018
ms.author: maggies
ms.openlocfilehash: 943e81c8c49a4a0707ed41b593093fc27a85a01e
ms.sourcegitcommit: c8c126c1b2ab4527a16a4fb8f5208e0f7fa5ff5a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2019
ms.locfileid: "54295871"
---
# <a name="install-power-bi-desktop-optimized-for-power-bi-report-server"></a>Instalar o Power BI Desktop otimizado para o Servidor de Relatório do Power BI
Saiba como instalar o Power BI Desktop otimizado para o Servidor de Relatório do Power BI.

Para criar relatórios do Power BI para o Servidor de Relatórios do Power BI você precisa baixar e instalar o Power BI Desktop otimizado para o Servidor de Relatórios do Power BI. Essa versão é diferente do Power BI Desktop usado com o serviço do Power BI. Por exemplo, a versão do Power BI Desktop para o serviço do Power BI inclui a versão prévia dos recursos que só ficam disponíveis na versão do Servidor de Relatórios do Power BI após serem liberados. Usar essa versão garante que o servidor de relatórios pode interagir com uma versão conhecida dos relatórios e do modelo. 

A boa notícia é que você pode instalar o Power BI Desktop e o Power BI Desktop otimizado para o Servidor de Relatórios do Power BI lado a lado no mesmo computador.

## <a name="download-and-install-power-bi-desktop"></a>Baixar e instalar o Power BI Desktop

A maneira mais fácil de ter certeza que você tem a versão mais recente do Power BI Desktop otimizado para o Servidor de Relatórios do Power BI é iniciar a partir do portal da Web do seu servidor de relatórios.

1. No portal da Web do servidor de relatórios, selecione a seta **Baixar** > **Power BI Desktop**.

    ![Baixe o Power BI Desktop no portal da Web](media/install-powerbi-desktop/report-server-download-web-portal.png)

    Ou você pode acessar diretamente o [Microsoft Power BI Desktop](https://www.microsoft.com/download/details.aspx?id=57271) (Otimizado para o Servidor de Relatórios do Microsoft Power BI – agosto de 2018) no Centro de Download da Microsoft.

2. Na página do Centro de Download, selecione **Baixar**.

3. Dependendo do seu computador, selecione: 

    - **PBIDesktopRS.msi** (a versão de 32 bits) ou

    - **PBIDesktopRS_x64.msi** (a versão de 64 bits).

1. Depois de baixar o instalador, execute o Assistente de Instalação do Power BI Desktop (agosto de 2018).

2. No final da instalação, marque **Iniciar o Power BI Desktop agora**.
   
    Ele é iniciado automaticamente e você está pronto para começar.

## <a name="verify-you-are-using-the-correct-version"></a>Verifique se você está usando a versão correta
É possível verificar se você está usando o Power BI Desktop correto examinando a tela de inicialização ou a barra de título no Power BI Desktop. A barra de título indica o mês de lançamento e o ano da versão.

![Barra de título do Power BI Desktop otimizada para o Servidor de Relatórios do Power BI](media/install-powerbi-desktop/power-bi-report-server-desktop-august-2018.png)

A versão do Power BI Desktop para o serviço do Power BI não possui o mês nem o ano na barra de título.

## <a name="file-extension-association"></a>Associação de extensão de arquivo
Se você instalou o Power BI Desktop e o Power BI Desktop otimizado para o Servidor de Relatório do Power BI no mesmo computador, a última instalação do Power BI Desktop terá a associação de arquivo com .pbix. Isso significa que quando você clicar duas vezes em um arquivo pbix, ele iniciará o Power BI Desktop instalado pela última vez.

Se você tinha o Power BI Desktop e, em seguida, instalou o Power BI Desktop otimizado para o Servidor de Relatório do Power BI, todos os arquivos pbix serão abertos no Power BI Desktop otimizado para o Servidor de Relatório do Power BI por padrão. Se, em vez disso, você preferir que o Power BI Desktop seja o padrão para iniciar ao abrir um arquivo pbix, reinstale o Power BI Desktop do serviço do Power BI.

Sempre é possível abrir a versão do Power BI Desktop que você deseja usar primeiro. E, em seguida, abra o arquivo no Power BI Desktop.

Editar um relatório do Power BI no Servidor de Relatório do Power BI ou criar um novo relatório do Power BI no portal da Web sempre abrirá a versão correta do Power BI Desktop.

## <a name="considerations-and-limitations"></a>Considerações e limitações
Os relatórios do Power BI no Servidor de Relatórios do Microsoft Power BI e no serviço do Power BI (http://app.powerbi.com), assim como nos aplicativos móveis do Power BI) agem praticamente da mesma maneira, mas alguns recursos são diferentes.

### <a name="in-a-browser"></a>Em um navegador
Os relatórios do Servidor de Relatório do Power BI dão suporte a todas as visualizações, inclusive:

* Elementos visuais personalizados

Os relatórios do Servidor de Relatório do Power BI não dão suporte a:

* Visuais do R
* Mapas ArcGIS
* Trilhas
* Recursos de visualização do Power BI Desktop

### <a name="in-the-power-bi-mobile-apps"></a>Nos aplicativos móveis do Power BI
Os relatórios do Servidor de Relatório do Power BI dão suporte a toda a funcionalidade básica nos [aplicativos móveis do Power BI](../consumer/mobile/mobile-apps-for-mobile-devices.md), incluindo:

* [Layout de relatório de telefone](../desktop-create-phone-report.md): é possível otimizar um relatório para os aplicativos móveis do Power BI. Em seu telefone celular, os relatórios otimizados têm um ícone especial chamado ![Ícone de layout de relatório para telefone](media/install-powerbi-desktop/power-bi-rs-mobile-optimized-icon.png) e um layout.
  
    ![Relatórios otimizado para telefones](media/install-powerbi-desktop/power-bi-rs-mobile-optimized-report.png)

Os relatórios do Servidor de Relatório do Power BI não dão suporte a estes recursos nos aplicativos móveis do Power BI:

* Visuais do R
* Mapas ArcGIS
* Elementos visuais personalizados
* Trilhas
* Filtragem geográfica ou códigos de barra

## <a name="power-bi-desktop-for-earlier-versions-of-power-bi-report-server"></a>Power BI Desktop para versões anteriores do Servidor de Relatórios do Power BI

Se seu servidor de relatório é de uma versão anterior, você precisa da versão correspondente do Power BI Desktop. Aqui estão as duas versões anteriores.

- Microsoft Power BI Desktop ([otimizado para o Servidor de Relatórios do Power BI – outubro de 2017](https://www.microsoft.com/download/details.aspx?id=56136))
- Microsoft Power BI Desktop ([otimizado para o Servidor de Relatórios do Power BI – junho de 2017](https://www.microsoft.com/download/details.aspx?id=55330))

## <a name="next-steps"></a>Próximas etapas
Agora que o Power BI Desktop foi instalado, é possível começar a criar relatórios do Power BI.

[Criar um relatório do Power BI para o Servidor de Relatórios do Power BI](quickstart-create-powerbi-report.md)  
[O que é o Servidor de Relatórios do Power BI?](get-started.md)

Mais perguntas? [Experimente perguntar à Comunidade do Power BI](https://community.powerbi.com/)

