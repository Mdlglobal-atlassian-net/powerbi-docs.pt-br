---
title: Portal de administração do Power BI
description: O portal de administração permite o gerenciamento de locatário do Power BI em sua organização. Ele inclui itens como métricas de uso, acesso ao Centro de administração do Microsoft 365 e configurações.
author: mgblythe
ms.author: mblythe
manager: kfile
ms.reviewer: ''
ms.service: powerbi
ms.subservice: powerbi-admin
ms.topic: conceptual
ms.date: 05/20/2019
ms.custom: seodec18
LocalizationGroup: Administration
ms.openlocfilehash: 6c9d59bbc2c6bf81242166bef4cd7584f52fb633
ms.sourcegitcommit: 60dad5aa0d85db790553e537bf8ac34ee3289ba3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/29/2019
ms.locfileid: "65941601"
---
# <a name="administering-power-bi-in-the-admin-portal"></a>Como administrar o Power BI no portal de administração

O portal de administração permite que você gerencie um *locatário* do Power BI para sua organização. O portal inclui itens como métricas de uso, acesso ao centro de administração do Microsoft 365 e configurações.

O portal de administração completo é acessível a todos os usuários que sejam administradores globais no Office 365 ou que detenham a função de administrador de serviços do Power BI. Se você não estiver em uma dessas funções, verá apenas **Configurações de capacidade** no portal. Para obter mais informações sobre a função de administrador de serviços do Power BI, consulte [Noções básicas sobre a função de administrador do Power BI](service-admin-role.md).

## <a name="how-to-get-to-the-admin-portal"></a>Como obter o portal de administração

Sua conta deve ser marcada como **Administrador Global** no Office 365 ou no Azure Active Directory ou ter recebido a função de administrador de serviços do Power BI, para obter acesso ao portal de administração do Power BI. Para obter mais informações sobre a função de administrador de serviços do Power BI, consulte [Noções básicas sobre a função de administrador do Power BI](service-admin-role.md). Para acessar o portal de administração do Power BI, faça o seguinte:

1. Selecione a engrenagem de configurações na parte superior direita do serviço do Power BI.

1. Selecione **portal de Administração**.

    ![Configurações do portal de administração](media/service-admin-portal/powerbi-admin-settings.png)

Há nove guias no portal. O restante deste artigo fornece informações sobre cada uma dessas guias.

![Navegação do portal de administração](media/service-admin-portal/powerbi-admin-landing-page.png)

* [Métricas de uso](#usage-metrics)
* [Usuários](#users)
* [Logs de auditoria](#audit-logs)
* [Configurações de locatário](#tenant-settings)
* [Configurações de capacidade](#capacity-settings)
* [Códigos de inserção](#embed-codes)
* [Elementos visuais da organização](#organization-visuals)
* [Fluxo de dados armazenamento (visualização)](#dataflowStorage)
* [Workspaces](#workspaces)

## <a name="usage-metrics"></a>Métricas de uso

As **Métricas de uso** permitem que você monitore o uso do Power BI para sua organização. Ele também fornece a capacidade de ver quais usuários e grupos são mais ativos no Power BI para sua organização.

> [!NOTE]
> Na primeira vez que acessar o dashboard ou depois de visitar novamente após um longo período de não exibição do dashboard, você provavelmente encontrará uma tela de carregamento enquanto carregamos o dashboard.

Quando o painel for carregado, você verá duas seções de blocos. A primeira inclui os dados de uso de usuários individuais e a segunda seção tem informações semelhantes para os grupos em sua organização.

Aqui está uma análise do que você verá em cada bloco:

* Contagem distinta de todos os painéis, relatórios e conjuntos de dados no workspace do usuário
  
    ![Contagem distinta de painéis, relatórios e conjuntos de dados](media/service-admin-portal/powerbi-admin-usage-metrics-number-tiles.png)

* Painel mais consumido pelo número de usuários que podem acessá-lo. Por exemplo, se você tem um painel que compartilhou com três usuários e também o adiciona a um pacote de conteúdo com dois usuários diferentes conectados a ele, sua contagem é de 6 (1 + 3 + 2)
  
    ![Painéis mais consumidos](media/service-admin-portal/powerbi-admin-usage-metrics-top-dashboards.png)

* Os conteúdo mais populares aos quais os usuários estão conectados. Isso pode ser qualquer coisa que os usuários podem acessar através do processo Obter Dados, portanto, pacotes de conteúdo SaaS, pacotes de conteúdo organizacional, arquivos ou bancos de dados de conteúdo.
  
    ![Pacotes mais consumidos](media/service-admin-portal/powerbi-admin-usage-metrics-top-connections.png)

* Uma exibição de seus principais usuários sobre quantos painéis eles têm, incluindo painéis criados por eles mesmos e painéis compartilhados com eles.
  
    ![Principais usuários – painéis](media/service-admin-portal/powerbi-admin-usage-metrics-top-users-dashboards.png)

* Uma exibição de seus principais usuários com base em quantos relatórios eles têm
  
    ![Principais usuários – relatórios](media/service-admin-portal/powerbi-admin-usage-metrics-top-users-reports.png)

A segunda seção mostra o mesmo tipo de informação, mas com base em grupos. Isso permite que você veja quais grupos em sua organização são mais ativos e os tipos de conteúdos que estão consumindo.

Com essas informações, você fica sabendo como as pessoas estão usando o Power BI em toda a organização e consegue reconhecer esses usuários e grupos que são muito ativos na organização.

## <a name="users"></a>Usuários

O gerenciamento de administradores, grupos e usuários do Power BI é feito no Centro de administração do Microsoft 365. A guia **Usuários** fornece um link para o centro de administração para seu locatário.

![Ir para o Centro de administração do Microsoft 365](media/service-admin-portal/powerbi-admin-manage-users.png)

## <a name="audit-logs"></a>Logs de auditoria

O gerenciamento dos logs de auditoria do Power BI é feito na Central de Segurança e Conformidade do Office 365. A guia **Logs de auditoria** fornece um link para a Central de Segurança e Conformidade para seu locatário. [Saiba mais](service-admin-auditing.md)

Para usar os logs de auditoria, verifique se a configuração [**Criar logs de auditoria para conformidade e auditoria de atividade interna** ](#create-audit-logs-for-internal-activity-auditing-and-compliance) está habilitada.

## <a name="tenant-settings"></a>Configurações de locatário

A guia **Configurações de locatário** possibilita um controle refinado sobre os recursos disponibilizados para sua organização. Se você tiver dúvidas relacionadas a dados confidenciais, talvez alguns dos nossos recursos não sejam adequados para sua organização, ou talvez você queira apenas que um recurso em particular esteja disponível para um grupo específico.

A imagem a seguir mostra as duas primeiras seções da guia **Configurações de locatário**.

![Configurações de locatário](media/service-admin-portal/powerbi-admin-tenant-settings.png)

> [!NOTE]
> Pode levar até 10 minutos para que uma alteração de configuração entre em vigor para todos em seu locatário.

As configurações podem ter três estados:

* **Desabilitado para toda a organização**: ninguém na sua organização pode usar esse recurso.

    ![Configuração desabilitado para todos](media/service-admin-portal/powerbi-admin-tenant-settings-disabled.png)

* **Habilitado para toda a organização**: todos em sua organização podem usar esse recurso.

    ![Configuração habilitado para todos](media/service-admin-portal/powerbi-admin-tenant-settings-enabled.png)

* **Habilitado para um subconjunto da organização**: um subconjunto específico de usuários ou grupos em sua organização pode usar o recurso.

    Você pode habilitar o recurso para toda a organização, exceto para um grupo específico de usuários.

    ![Configuração habilitado para um subconjunto](media/service-admin-portal/powerbi-admin-tenant-settings-enabled-except.png)

    Também é possível habilitar o recurso apenas para um grupo específico de usuários e também desabilitá-lo para um grupo de usuários. O uso dessa abordagem garante que determinados usuários não tenham acesso ao recurso mesmo que estejam no grupo permitido.

    ![Configuração habilitado com exceção](media/service-admin-portal/powerbi-admin-tenant-settings-enabled-except2.png)

As próximas seções fornecem uma visão geral dos diferentes tipos de configurações de locatário.

## <a name="help-and-support-settings"></a>Ajuda e suporte a configurações

### <a name="publish-get-help-information"></a>Publicar as informações de "Ajuda"

Os usuários da organização podem ir para a Ajuda interna e dar suporte a recursos no menu Ajuda do Power BI. Especificamente, esses parâmetros altera o comportamento dos itens de menu de ajuda Get, comunidade e saiba mais.

Também é possível especificar uma URL para direcionar usuários a uma solução personalizada para solicitações de licenciamento. Esse parâmetro personaliza a URL de destino do botão de atualização de conta que um usuário sem uma licença do Power BI Pro pode encontrar na atualização para a caixa de diálogo do Power BI Pro, bem como na página Gerenciar armazenamento pessoal.

## <a name="workspace-settings"></a>Configurações do workspace

### <a name="create-workspaces"></a>Criar espaços de trabalho

Os administradores usam o **criar espaços de trabalho** configuração para indicar quais usuários na organização podem criar espaços de trabalho de aplicativo para colaborar em dashboards, relatórios e outro conteúdo. Saiba mais sobre [espaços de trabalho do aplicativo](service-create-the-new-workspaces.md).

O portal de administração tem outra seção de configurações sobre os espaços de trabalho em seu locatário. Nesta seção, você pode classificar e filtrar a lista de espaços de trabalho e exibir os detalhes de cada espaço de trabalho. Ver [espaços de trabalho](#workspaces) para obter detalhes.

No portal de administração, você também controlar quais usuários têm permissões para distribuir aplicativos para a organização. Ver [publicar aplicativos e pacotes de conteúdo em toda a organização](#publish-content-packs-and-apps-to-the-entire-organization) neste artigo para obter detalhes.

## <a name="export-and-sharing-settings"></a>Configurações de exportação e compartilhamento

### <a name="share-content-with-external-users"></a>Compartilhar conteúdo com usuários externos

Os usuários da organização podem compartilhar dashboards com usuários fora da organização. [Saiba mais](service-share-dashboards.md#share-a-dashboard-or-report-with-people-outside-your-organization)

![Configuração de usuários externos](media/service-admin-portal/powerbi-admin-sharing-external-02.png)

A imagem a seguir mostra a mensagem exibida quando você compartilha com um usuário externo.

![Compartilhar com usuário externo](media/service-admin-portal/powerbi-admin-sharing-external.png)  

### <a name="publish-to-web"></a>Publicar na Web

Os usuários na organização podem publicar relatórios na Web. [Saiba mais](service-publish-to-web.md)

A imagem a seguir mostra o menu **Arquivo** de um relatório quando a configuração **Publicar na Web** está habilitada.

![Configuração Publicar na Web](media/service-admin-portal/powerbi-admin-publish-to-web.png)

Os usuários veem diferentes opções na interface do usuário a depender do local onde se encontra a configuração de **Publicar na Web**.

|Recurso |Habilitado para toda a organização |Desabilitado para toda a organização |Especificar grupos de segurança   |
|---------|---------|---------|---------|
|**Publicar na Web** no menu **Arquivo** do relatório.|Habilitado para todos|Não visível para todos|Visível somente para usuários ou grupos autorizados.|
|**Gerenciar códigos de inserção** em **Configurações**|Habilitado para todos|Habilitado para todos|Habilitado para todos<br><br>Opção * **Excluir** somente para usuários ou grupos autorizados.<br>* **Obter códigos** habilitados para todos.|
|**Códigos de inserção** no portal de administração|O status refletirá uma das seguintes opções:<br>* Ativo<br>* Sem suporte<br>* Bloqueado|O status é exibido como **desabilitado**|O status refletirá uma das seguintes opções:<br>* Ativo<br>* Sem suporte<br>* Bloqueado<br><br>Se um usuário não estiver autorizado conforme a configuração do locatário, o status exibirá **violado**.|
|Relatórios publicados existentes|Tudo habilitado|Tudo desabilitado|Os relatórios continuam a ser renderizados para todos.|

### <a name="export-data"></a>Exportar dados

Os usuários na organização podem exportar dados de um bloco ou visualização. [Saiba mais](visuals/power-bi-visualization-export-data.md)

A imagem a seguir mostra a opção para exportar dados de um bloco.

![Exportar dados de um bloco](media/service-admin-portal/powerbi-admin-export-data.png)

> [!NOTE]
> Desabilitar a opção **Exportar dados** também impede os usuários de usar o recurso **Analisar no Excel**, bem como de usar a conexão dinâmica do serviço do Power BI.

### <a name="export-reports-as-powerpoint-presentations-or-pdf-documents"></a>Exportar relatórios como apresentações do PowerPoint ou documentos PDF

Os usuários da organização podem exportar relatórios do Power BI como arquivos do PowerPoint ou documentos PDF. [Saiba mais](consumer/end-user-powerpoint.md)

A imagem a seguir mostra o menu **Arquivo** de um relatório quando a configuração **Exportar relatórios como apresentações do PowerPoint ou documentos PDF** está habilitada.

![Exportar relatórios como apresentações do PowerPoint](media/service-admin-portal/powerbi-admin-powerpoint.png)

### <a name="print-dashboards-and-reports"></a>Imprimir painéis e relatórios

Os usuários na organização podem imprimir dashboards e relatórios. [Saiba mais](consumer/end-user-print.md)

A imagem a seguir mostra a opção para imprimir um painel.

![Imprimir dashboard](media/service-admin-portal/powerbi-admin-print-dashboard.png)

A imagem a seguir mostra o menu **Arquivo** de um relatório quando a configuração **Imprimir painéis e relatórios** está habilitada.

![Imprimir relatório](media/service-admin-portal/powerbi-admin-print-report.png)

### <a name="allow-external-guest-users-to-edit-and-manage-content-in-the-organization"></a>Permitir que os usuários externos convidados editem e gerenciem o conteúdo da organização
Os usuários convidados B2B do Azure podem editar e gerenciar conteúdo na organização. [Saiba mais](service-admin-azure-ad-b2b.md)

A imagem a seguir mostra a opção de permitir que os usuários externos convidados editem e gerenciem o conteúdo da organização.

![Permitir que os usuários externos convidados editem e gerenciem o conteúdo da organização](media/service-admin-portal/powerbi-admin-tenant-settings-b2b-guest-edit-manage.png)

## <a name="content-pack-and-app-settings"></a>Configurações de aplicativo e pacote de conteúdo

### <a name="publish-content-packs-and-apps-to-the-entire-organization"></a>Publicar aplicativos e pacotes de conteúdo em toda a organização

Admins. use essa configuração para decidir quais usuários podem publicar pacotes de conteúdo e aplicativos a toda a organização, em vez de apenas determinados grupos. Saiba mais sobre [publicação de aplicativos](service-create-distribute-apps.md).

A imagem a seguir mostra a opção **Minha organização inteira** durante a criação de um pacote de conteúdo.

![Publicar o pacote de conteúdo na organização](media/service-admin-portal/powerbi-admin-publish-entire-org.png)

### <a name="create-template-apps-and-organizational-content-packs"></a>Criar modelo de aplicativos e pacotes de conteúdo organizacional

Os usuários na organização podem criar aplicativos de modelo e os pacotes de conteúdo organizacional que usam conjuntos de dados criados em uma fonte de dados no Power BI Desktop. Saiba mais sobre [aplicativos de modelo](template-content-pack-authoring.md).

### <a name="push-apps-to-end-users"></a>Enviar aplicativos por push para usuários finais

Criadores de relatório podem compartilhar aplicativos diretamente com os usuários finais sem exigir a instalação do [AppSource](https://appsource.microsoft.com). Saiba mais sobre [instalar aplicativos automaticamente para os usuários finais](service-create-distribute-apps.md#automatically-install-apps-for-end-users).

## <a name="integration-settings"></a>Configurações de integração

### <a name="ask-questions-about-data-using-cortana"></a>Faça perguntas sobre dados usando a Cortana

Os usuários na organização podem fazer perguntas sobre seus dados usando a Cortana. [Saiba mais](service-cortana-enable.md)

> [!NOTE]
> Essa configuração se aplica a toda a organização e não pode ser limitada a grupos específicos.

### <a name="use-analyze-in-excel-with-on-premises-datasets"></a>Usar a opção Analisar no Excel com conjuntos de dados locais

Os usuários na organização podem usar o Excel para exibir e interagir com conjuntos de dados locais do Power BI. [Saiba mais](service-analyze-in-excel.md)

> [!NOTE]
> Desabilitar a opção **Exportar Dados** também impede os usuários de usar o recurso **Analisar no Excel**.

### <a name="use-arcgis-maps-for-power-bi"></a>Usar o ArcGIS Maps for Power BI

Os usuários na organização podem usar a visualização do ArcGIS Maps for Power BI, fornecida pela Esri. [Saiba mais](visuals/power-bi-visualization-arcgis.md)

### <a name="use-global-search-for-power-bi-preview"></a>Usar a pesquisa global para o Power BI (versão prévia)

Os usuários na organização podem usar recursos de pesquisa externos que se baseiam no Azure Search. Por exemplo, eles podem usar a Cortana para recuperar informações importantes diretamente dos relatórios e dashboards do Power BI. [Saiba mais](service-cortana-intro.md)

## <a name="custom-visuals-settings"></a>Configurações visuais personalizadas

### <a name="add-and-use-custom-visuals"></a>Adicionar e usar visuais personalizados

Os usuários na organização podem interagir com e compartilhar elementos visuais personalizados. [Saiba mais](power-bi-custom-visuals.md)

> [!NOTE]
> Essa configuração pode ser aplicada a toda a organização ou limitada a grupos específicos.


O Power BI Desktop (a partir da versão de março de 2019) dá suporte ao uso da **Política de Grupo** para desabilitar o uso de visuais personalizados nos computadores implantados de uma organização.

<table>
<tr><th>Atributo</th><th>Valor</th>
</tr>
<td>chave</td>
    <td>Software\Políticas\Microsoft\Power BI Desktop\</td>
<tr>
<td>valueName</td>
<td>EnableCustomVisuals</td>
</tr>
</table>

Um valor de 1 (decimal) habilita o uso de visuais personalizados no Power BI (esse é o padrão).

Um valor de 0 (decimal) desabilita o uso de visuais personalizados no Power BI.

### <a name="allow-only-certified-visuals"></a>Permitir somente visuais certificados

Os usuários da organização que receberam permissões para adicionar e usar visuais personalizados, indicado pela configuração "Adicionar e usar visuais personalizados", só poderão usar [visuais personalizados certificados](https://go.microsoft.com/fwlink/?linkid=2002010) (os visuais não certificados serão bloqueados e exibirão uma mensagem de erro quando usados). 


O Power BI Desktop (a partir da versão de março de 2019) dá suporte ao uso da **política de grupo** para desabilitar o uso de visuais personalizados não certificados nos computadores implantados de uma organização.

<table>
<tr><th>Atributo</th><th>Valor</th>
</tr>
<td>chave</td>
    <td>Software\Políticas\Microsoft\Power BI Desktop\</td>
<tr>
<td>valueName</td>
<td>EnableUncertifiedVisuals</td>
</tr>
</table>

Um valor de 1 (decimal) habilita o uso de visuais personalizados não certificados no Power BI (esse é o padrão).

Um valor de 0 (decimal) desabilita o uso de visuais personalizados não certificados no Power BI (essa opção permite somente o uso de [visuais personalizados certificados](https://go.microsoft.com/fwlink/?linkid=2002010)).

## <a name="r-visuals-settings"></a>Configurações de elementos visuais do R

### <a name="interact-with-and-share-r-visuals"></a>Interagir e compartilhar visuais do R

Os usuários na organização podem interagir e compartilhar elementos visuais criados com scripts do R. [Saiba mais](visuals/service-r-visuals.md)

> [!NOTE]
> Essa configuração se aplica a toda a organização e não pode ser limitada a grupos específicos.

## <a name="audit-and-usage-settings"></a>Configurações de auditoria e de uso

### <a name="create-audit-logs-for-internal-activity-auditing-and-compliance"></a>Criar logs de auditoria para conformidade e auditoria de atividade interna

Os usuários na organização podem usar a auditoria para monitorar as ações executadas no Power BI por outros usuários na organização. [Saiba mais](service-admin-auditing.md)

Essa configuração deve ser habilitada para que as entradas de log de auditoria sejam registradas. Pode haver um atraso de até 48 horas entre a habilitação da auditoria e a possibilidade de exibir dados de auditoria. Se os dados não forem exibidos imediatamente, verifique os logs de auditoria mais tarde. Pode haver um atraso semelhante entre a obtenção da permissão para exibir os logs de auditoria e a possibilidade de acessá-los.

> [!NOTE]
> Essa configuração se aplica a toda a organização e não pode ser limitada a grupos específicos.

### <a name="usage-metrics-for-content-creators"></a>Métricas de uso para criadores de conteúdo

Os usuários na organização podem ver métricas de uso para painéis e relatórios que eles criaram. [Saiba mais](service-usage-metrics.md)

### <a name="per-user-data-in-usage-metrics-for-content-creators"></a>Dados por usuário em métricas de uso para criadores de conteúdo

As métricas de uso para criadores de conteúdo expõem os nomes de exibição e os endereços de email dos usuários que estão acessando o conteúdo. [Saiba mais](service-usage-metrics.md)

Os dados por usuário são habilitados para as métricas de uso, por padrão, e as informações de conta do criador do conteúdo estão incluídas no relatório de métricas. Se você não quiser incluir essa informação para alguns ou todos os usuários, desabilite o recurso para grupos de segurança especificados ou para toda a organização. Em seguida, as informações da conta serão mostradas no relatório como *Sem nome*.

## <a name="dashboard-settings"></a>Configurações do dashboard

### <a name="data-classification-for-dashboards"></a>Classificação de dados para dashboards

Os usuários na organização podem marcar painéis com classificações indicando os níveis de segurança do painel. [Saiba mais](service-data-classification.md)

> [!NOTE]
> Essa configuração se aplica a toda a organização e não pode ser limitada a grupos específicos.

## <a name="developer-settings"></a>Configurações do desenvolvedor

### <a name="embed-content-in-apps"></a>Inserir conteúdo em aplicativos

Usuários da organização podem inserir relatórios e dashboards do Power BI em aplicativos de SaaS (software como serviço). Desabilitar essa configuração impede os usuários de usar as APIs REST para inserir conteúdo do Power BI em seus aplicativos. [Saiba mais](developer/embedding.md)

### <a name="allow-service-principals-to-use-power-bi-apis"></a>Permitir que as entidades de serviço usem APIs do Power BI

Aplicativos Web registrados no Azure Active Directory (Azure AD) usará uma entidade de serviço atribuída para acessar APIs do Power BI sem um usuário conectado. Para permitir que um aplicativo para usar a autenticação de entidade de serviço sua entidade de serviço deve ser incluído em um grupo de segurança permitidos. [Saiba mais](developer/embed-service-principal.md)

> [!NOTE]
> As entidades de serviço herdam as permissões para todas as configurações de locatário do Power BI de seu grupo de segurança. Para restringir permissões, crie um grupo de segurança dedicado para entidades de serviço e adicione-o à lista "Exceto grupos de segurança específicos" para as configurações relevantes habilitadas do Power BI.

## <a name="dataflow-settings"></a>Configurações do fluxo de dados

### <a name="create-and-use-dataflows"></a>Criar e usar fluxos de dados

Os usuários na organização podem criar e usar fluxos de dados. Para obter uma visão geral dos fluxos de dados, consulte [preparação de dados de autoatendimento no Power BI](service-dataflows-overview.md). Para habilitar os fluxos de dados em uma capacidade Premium, consulte [Configurar cargas de trabalho](service-admin-premium-workloads.md).

> [!NOTE]
> Essa configuração se aplica a toda a organização e não pode ser limitada a grupos específicos.

## <a name="template-apps-settings-preview"></a>Configurações do aplicativo de modelo (versão prévia)

Duas configurações controlam os aplicativos de modelo. 

![Configurações de aplicativos de modelo do portal de administração do Power BI](media/service-admin-portal/power-bi-admin-portal-template-apps.png)

### <a name="create-template-apps-preview"></a>Criar Aplicativos de Modelo (versão prévia)

Os usuários na organização podem criar aplicativos de modelo. Os criadores de aplicativos de modelo, em seguida, podem distribuí-los aos clientes fora da sua organização por meio de [AppSource](https://appsource.microsoft.com) ou outros métodos de distribuição.

![Portal de administração do Power BI, configuração Criar aplicativos de modelo](media/service-admin-portal/power-bi-admin-portal-template-app-settings.png)

### <a name="install-template-apps-preview"></a>Instalar aplicativos de modelo (visualização)

Os usuários da organização podem baixar e instalar o modelo de aplicativos [AppSource](https://appsource.microsoft.com) ou de outra fonte.

> [!NOTE]
> Essa configuração determina quais usuários podem instalar aplicativos de modelo em suas contas do Power BI.

## <a name="capacity-settings"></a>Configurações de capacidade

### <a name="power-bi-premium"></a>Power BI Premium

A guia **Power BI Premium** permite que você gerencie qualquer capacidade do Power BI Premium (SKU EM ou P) que tenha sido comprada para sua organização. Todos os usuários na organização podem ver a guia **Power BI Premium**, mas só verão conteúdo nela se forem atribuídos como *Administradores de capacidade* ou se forem um usuário com permissões de atribuição. Se um usuário não tiver nenhuma permissão, a mensagem de erro a seguir será exibida.

![Sem acesso às configurações Premium](media/service-admin-portal/premium-settings-no-access.png)

### <a name="power-bi-embedded"></a>Power BI Embedded

A guia **Power BI Embedded** permite que você exiba suas capacidades do Power BI Embedded (SKU A) que comprou para o cliente. Uma vez que você só poderá comprar um SKUs do Azure, você [gerenciar capacidades incorporadas no Azure](developer/azure-pbie-create-capacity.md) partir **portal do Azure**.

Para saber mais sobre como gerenciar as configurações do Power BI Embedded (SKU A), confira [O que é o Power BI Embedded](developer/azure-pbie-what-is-power-bi-embedded.md).

## <a name="embed-codes"></a>Códigos de inserção

Como administrador, você pode exibir os códigos de inserção que são gerados para seu locatário. Você também pode revogar ou excluir códigos. [Saiba mais](service-publish-to-web.md)

![Códigos de inserção dentro do portal de administração do Power BI](media/service-admin-portal/embed-codes.png)

## <a name="organizational-visuals">Elementos visuais da organização</a>

A guia **Elementos visuais da organização** permite implantar e gerenciar elementos visuais personalizados dentro da sua organização. Com elementos visuais da organização, você pode implantar visuais proprietários em sua organização, que os autores de relatório podem, em seguida, descobrir e importar em seus relatórios do Power BI Desktop. [Saiba mais](power-bi-custom-visuals-organization.md)

> [!WARNING]
> Um elemento visual personalizado pode conter código com riscos de segurança ou privacidade; verifique se você confia no autor e a fonte do visual personalizado antes de implantá-lo no repositório da organização.

A imagem a seguir mostra todos os elementos visuais personalizados que estão implantados no momento no repositório da organização.

![Visual de administrador da organização](media/service-admin-portal/power-bi-custom-visuals-organizational-admin-01.png)

### <a name="add-a-new-custom-visual"></a>Adicionar um novo elemento visual personalizado

Para adicionar um novo elemento visual personalizado à lista, siga estas etapas. 

1. No painel direito, selecione **Adicionar um visual personalizado**.

    ![Formulário dos visuais personalizados](media/service-admin-portal/power-bi-custom-visuals-organizational-admin-02.png)

1. Preencha o formulário **Adicionar visual personalizado**:

    * **Escolha um arquivo .pbiviz** (obrigatório): selecione um arquivo de elemento visual personalizado para carregar. Apenas os elementos visuais personalizados da API com controle de versão têm suporte (leia aqui o que isso significa).

    Antes de carregar um elemento visual personalizado, você deve examinar tal elemento visual em relação à segurança e à privacidade, para verificar se ele se ajusta aos padrões da sua organização.

    * **Nomeie os elementos visuais personalizados** (obrigatório): dê um título curto para o elemento visual para que os usuários do Power BI Desktop compreendam facilmente o que ele faz

    * **Ícone**: o arquivo de ícone que é mostrado na interface do usuário do Power BI Desktop.

    * **Descrição**: uma breve descrição do elemento visual para fornecer mais contexto e treinamento para o usuário

1. Selecione **Adicionar** para iniciar a solicitação de carregamento. Se for bem-sucedido, você poderá ver o novo item na lista. Se falhar, você poderá receber uma mensagem de erro apropriada

### <a name="delete-a-custom-visual-from-the-list"></a>Exclua um visual personalizado da lista

Para excluir permanentemente o visual, selecione o ícone de lixeira para o visual no repositório.

> [!IMPORTANT]
> A exclusão é irreversível. Depois de excluído, o elemento visual interrompe imediatamente a renderização em relatórios existentes. Mesmo se você carregar o mesmo elemento visual novamente, ele não substituirá o anterior que foi excluído. No entanto, os usuários podem importar o novo elemento visual novamente e substituir a instância que eles têm em seus relatórios.

### <a name="disable-a-custom-visual-in-the-list"></a>Desabilitar um visual personalizado na lista

Para desabilitar o visual do repositório organizacional, selecione o ícone de engrenagem. Na seção **Acesso**, desabilite o visual personalizado.

Depois que você desabilitar o visual, ele não será renderizado em relatórios existentes e exibirá a mensagem de erro abaixo.

*Este visual personalizado não está mais disponível. Entre em contato com o administrador para obter detalhes.*

No entanto, os elementos visuais marcados com um indicador ainda funcionam.

Após qualquer alteração de atualização ou de administrador, os usuários do Power BI Desktop devem reiniciar o aplicativo ou atualizar o navegador no serviço do Power BI para ver as atualizações.

### <a name="update-a-visual"></a>Atualizar um elemento visual

Para atualizar o visual do repositório organizacional, selecione o ícone de engrenagem. Procure e carregue uma nova versão do elemento visual.

Verifique se a ID do Visual permanece inalterada. O novo arquivo substitui o arquivo anterior em todos os relatórios de toda a organização. No entanto, se a nova versão do visual prejudicar qualquer estrutura de dados de uso da versão anterior do visual, não substitua a versão anterior. Em vez disso, crie uma nova lista para a nova versão do visual. Por exemplo, adicione um novo número de versão (versão X.X) ao título do novo visual listado. Desse modo, fica claro que é o mesmo visual, apenas com um número de versão atualizada, assim os relatórios existentes não prejudicam a funcionalidade. Novamente, verifique se a ID do Visual permanece inalterada. Assim, na próxima vez que os usuários inserirem o repositório da organização do Power BI Desktop, poderão importar a nova versão, que pedirá que substituam a versão atual que têm no relatório.

Para saber mais, acesse [Frequently asked questions about organizational custom visuals](https://docs.microsoft.com/power-bi/power-bi-custom-visuals-faq#organizational-custom-visuals) (Perguntas frequentes sobre os visuais personalizados de organização)

## <a name="dataflowStorage">Fluxo de dados armazenamento (visualização)</a>

Por padrão, os dados usados com o Power BI são armazenados no armazenamento interno fornecido pelo Power BI. Com a integração de fluxos de dados e o Azure Data Lake Storage Gen2 (ADLS Gen2), você pode armazenar seus fluxos de dados na conta do Azure Data Lake Storage Gen2 da sua organização. Para saber mais, confira [Integração entre fluxos de dados e o Azure Data Lake (versão prévia)](service-dataflows-azure-data-lake-integration.md).

## <a name="workspaces"></a>Workspaces

Como administrador, você pode exibir os workspaces que existem em seu locatário. É possível classificar e filtrar a lista de workspaces e exibir os detalhes de cada um deles. As colunas da tabela correspondem às propriedades retornadas pela [API de Rest do administrador do Power BI](/rest/api/power-bi/admin) para espaços de trabalho. Espaços de trabalho pessoais são do tipo **PersonalGroup**, os espaços de trabalho clássicos são do tipo **grupo**, e os espaços de trabalho de experiência do novo espaço de trabalho são do tipo **espaço de trabalho**. Para obter mais informações, consulte [criar novos espaços de trabalho no Power BI](service-create-the-new-workspaces.md).

![Lista de workspaces](media/service-admin-portal/workspaces-list.png)


## <a name="next-steps"></a>Próximas etapas

[Administração do Power BI em sua organização](service-admin-administering-power-bi-in-your-organization.md)  
[Noções básicas sobre a função de administrador do Power BI](service-admin-role.md)  
[Auditoria do Power BI em sua organização](service-admin-auditing.md)  

Mais perguntas? [Experimente perguntar à Comunidade do Power BI](https://community.powerbi.com/)
