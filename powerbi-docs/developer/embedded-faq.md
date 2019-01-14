---
title: Perguntas frequentes sobre o Power BI Embedded
description: Navegue por uma lista de perguntas frequentes e respostas sobre o Power BI Embedded.
author: markingmyname
ms.author: maghan
manager: kfile
ms.reviewer: ''
ms.service: powerbi
ms.component: powerbi-developer
ms.topic: conceptual
ms.date: 12/20/2018
ms.openlocfilehash: 106d971a06777f7d22d1fb3cd2ba3995b95a21d9
ms.sourcegitcommit: b3af4f7ef486c95cea173caea5a31d0472816ddd
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/09/2019
ms.locfileid: "54136635"
---
# <a name="frequently-asked-questions-about-power-bi-embedded"></a>Perguntas frequentes sobre o Power BI Embedded

* Se você tiver outras dúvidas, [experimente perguntar à comunidade do Power BI](http://community.powerbi.com/).
* Ainda tem um problema? Acesse a [página de suporte do Power BI](https://powerbi.microsoft.com/support/).

## <a name="general"></a>Geral

### <a name="what-is-power-bi-embedded"></a>O que é o Power BI Embedded?

O Microsoft Power BI Embedded (PBIE) permite que os desenvolvedores de aplicativos insiram relatórios incríveis e totalmente interativos em aplicativos, sem o tempo e a despesa da criação de controles e de visualizações de dados desde o início.

### <a name="who-is-the-target-audience-for-power-bi-embedded"></a>Quem é o público-alvo do Power BI Embedded?

Os desenvolvedores e as empresas de software que fazem aplicativos próprios, conhecidas como ISVs (fornecedores independentes de software).

### <a name="how-is-power-bi-embedded-different-from-power-bi-the-service"></a>Qual a diferença entre o Power BI Embedded e o serviço do Power BI?

O Power BI Embedded é destinado aos ISVs ou aos desenvolvedores que criam aplicativos e desejam inserir elementos visuais neles para ajudar seus clientes a tomar decisões sem precisar criar uma solução de análise desde o início. A análise inserida permite que os usuários empresariais acessem os dados corporativos e executem consultas para gerar informações usando esses dados no aplicativo.

O Power BI é uma solução de análise de software como serviço que fornece às organizações uma exibição única dos dados corporativos mais críticos.

### <a name="what-is-the-difference-between-power-bi-premium-and-power-bi-embedded"></a>Qual é a diferença entre o Power BI Premium e o Power BI Embedded?

A capacidade do Power BI Premium é direcionada a empresas que desejam uma solução de BI completa para fornecer uma exibição única da organização, dos parceiros, dos clientes e dos fornecedores. O Power BI Premium ajuda a organização na tomada de decisões. O Power BI Premium é um produto SaaS que permite aos usuários consumir conteúdo por meio do portal do Power BI, de aplicativos móveis e de aplicativos desenvolvidos internamente.

O Power BI Embedded é destinado aos ISVs ou aos desenvolvedores que criam aplicativos e desejam inserir elementos visuais neles. O Power BI Embedded ajuda os clientes a tomar decisões por ser destinado aos desenvolvedores de aplicativos, de modo que os clientes desses aplicativos, incluindo qualquer pessoa dentro ou fora da organização, podem consumir o conteúdo armazenado na capacidade do Power BI Embedded. O conteúdo da capacidade do Power BI Embedded não pode ser compartilhado por meio de publicação com um clique na Web nem no SharePoint, além de não ser compatível como os relatórios do SSRS.

### <a name="what-is-the-microsoft-recommendation-for-when-a-customer-should-buy-power-bi-premium-vs-power-bi-embedded"></a>Segundo a recomendação da Microsoft, quando os clientes devem comprar o Power BI Premium e quando devem comprar o Power BI Embedded?

A recomendação da Microsoft é que as empresas comprem o Power BI Premium (solução de BI de nuvem de autoatendimento de nível empresarial) e que os ISVs comprem o Power BI Embedded (componentes de análise inseridos habilitados para a nuvem). No entanto, não há restrições em relação a qual produto um cliente pode comprar.

Pode haver alguns casos em que um ISV (normalmente de grande porte) deseja usar uma SKU P para obter os benefícios adicionais do serviço do Power BI predefinido na organização, bem como inseri-los nos aplicativos. Algumas empresas poderão decidir usar. As SKUs A no Azure se só estiverem interessadas em criar aplicativos de linha de negócios e em inserir análise neles, e não em usar o serviço do Power BI predefinido.

### <a name="how-many-embed-tokens-can-i-create"></a>Quantos tokens inseridos posso criar?

Tokens inseridos com licença PRO destinam-se para teste de desenvolvimento, portanto, o número de tokens inseridos que uma conta mestre do Power BI pode gerar é limitado. Você deve [adquirir uma capacidade](#technical) para inserir em um ambiente de produção. Não há limites para a quantidade de tokens inseridos que você pode gerar quando uma capacidade é adquirida. Acesse [Recursos Disponíveis](https://docs.microsoft.com/rest/api/power-bi/availablefeatures) para verificar o valor de uso que indica o uso inserido atual, em percentual.

## <a name="technical"></a>Técnico

### <a name="what-is-the-difference-between-the-a-skus-in-azure-and-the-em-skus-in-office-365"></a>Qual é a diferença entre os SKUs A no Azure e os SKUs EM no Office 365?

O PowerBI.com é uma solução empresarial que inclui muitas funcionalidades, como colaboração social, assinatura de email, etc., em uma oferta de software como serviço

O Power BI Embedded é um conjunto de APIs disponíveis para os desenvolvedores criarem uma solução de análise inserida em uma oferta de plataforma como serviço. Para o cenário de análise inserida, o PowerBI.com deve ser usado para ajudar ISVs e desenvolvedores a gerenciar o conteúdo da solução de análise inserida deles e as configurações de nível de locatário.

Veja aqui uma lista parcial das diferenças que você pode usar com cada um deles.

| Recurso | Power BI Embedded | Capacidade do Power BI Premium | Capacidade do Power BI Premium |
|----------------------------------------------------------------------------------|-------------------|---------------------------|---------------------------|
|   | (SKUs A) | (SKUs EM) | (SKUs P) |
| Inserir artefatos de um workspace do aplicativo do Power BI | Capacidade do Azure | Capacidade do Office 365 | Capacidade do Office 365 |
| Consumir relatórios do Power BI em um aplicativo inserido | Sim | Sim | Sim |
| Consumir relatórios do Power BI no SharePoint | Não | Sim | Sim |
| Consumir relatórios do Power BI no Dynamics | Não | Sim | Sim |
| Consumir relatórios do Power BI no Teams (exceto aplicativo móvel) | Não | Sim | Sim |
| Acessar conteúdo com uma licença GRATUITA do Power BI no Powerbi.com e no Power BI Mobile | Não | Não | Sim |
| Acessar conteúdo com uma licença GRATUITA do Power BI inserida em aplicativos do MS Office | Não | Sim | Sim |

### <a name="power-bi-now-offers-three-skus-for-embedding-a-skus-em-skus-and-p-skus-which-one-should-i-purchase-for-my-scenario"></a>O Power BI agora oferece três SKUs para inserção: SKUs A, SKUs EM e SKUs P. Qual devo comprar para meu cenário?

|  |SKU A (Power BI Embedded)  |SKU EM (Power BI Premium)  |SKU P (Power BI Premium)  |
|---------|---------|---------|---------|
|Comprar  |Portal do Azure |Office |Office |
|Casos de uso | Inserir conteúdo em aplicativo próprio | <li> Inserir conteúdo em aplicativo próprio <br><br></br> <li> Inserir conteúdo em aplicativos do MS Office: <br> - [SharePoint](https://powerbi.microsoft.com/blog/integrate-power-bi-reports-in-sharepoint-online/) <br> - [Teams (exceto aplicativo móvel)](https://powerbi.microsoft.com/blog/power-bi-teams-up-with-microsoft-teams/) <br> - [Dynamics 365](https://docs.microsoft.com/dynamics365/customer-engagement/basics/add-edit-power-bi-visualizations-dashboard) | <li> Inserir conteúdo em aplicativo próprio <br><br></br> <li> Inserir conteúdo em aplicativos do MS Office: <br> - [SharePoint](https://powerbi.microsoft.com/blog/integrate-power-bi-reports-in-sharepoint-online/) <br> - [Teams (exceto aplicativo móvel)](https://powerbi.microsoft.com/blog/power-bi-teams-up-with-microsoft-teams/) <br> - [Dynamics 365](https://docs.microsoft.com/dynamics365/customer-engagement/basics/add-edit-power-bi-visualizations-dashboard) <br><br></br> <li> Compartilhar conteúdo com usuários do Power BI por meio do [serviço do Power BI](https://powerbi.microsoft.com/en-us/)  |
|Cobrança |A cada hora |Mensal |Mensal |
|Compromisso  |Sem compromisso |Anual  |Mensal/anual |
|Diferença |Elasticidade completa: pode aumentar/reduzir, pausar/retomar recursos no Portal do Azure ou por meio da API  |Pode ser usado para inserir conteúdo no SharePoint Online e no Microsoft Teams (exceto aplicativo móvel) |Combine inserção em aplicativos e use a mesma capacidade do serviço do Power BI |

### <a name="what-are-the-prerequisites-to-create-a-pbie-capacity-in-azure"></a>Quais são os pré-requisitos para criar uma capacidade de PBIE no Azure?

* Você precisa entrar no seu diretório organizacional (não há suporte para contas MSA).
* Você precisa ter um locatário do Power BI, isto é, pelo menos um usuário em seu diretório deve estar inscrito no Power BI. 
* Você precisa ter uma assinatura do Azure em seu diretório organizacional.

### <a name="how-can-i-monitor-power-bi-embedded-capacity-consumption"></a>Como posso monitorar o consumo de capacidade do Power BI Embedded?

* Usando o [portal do administrador do Power BI](../service-admin-portal.md#power-bi-embedded).

* Fazendo o download do [aplicativo de métricas](https://review.docs.microsoft.com/power-bi/service-admin-premium-monitor-capacity) no Power BI.

* Usando a [criação de log de diagnóstico do Azure](azure-pbie-diag-logs.md).

### <a name="will-my-capacity-scale-automatically-to-adjust-to-the-consumption-of-my-app"></a>Minha capacidade será dimensionada automaticamente para ajustar-se ao consumo de meu aplicativo?

Embora não haja dimensionamento automatizado no momento, todas as APIs podem ser dimensionadas a qualquer momento.

### <a name="why-creatingscalingresuming-a-capacity-results-in-putting-the-capacity-into-a-suspended-state"></a>Por que criar/dimensionar/retomar uma capacidade resulta na capacidade em um estado suspenso?

O provisionamento de uma capacidade (dimensionar/retomar/criar) pode falhar. O autor da chamada de provisionamento deve verificar o ProvisioningState de uma capacidade usando a API Obter detalhes: [Capacidades – Obter detalhes](https://docs.microsoft.com/rest/api/power-bi-embedded/capacities/getdetails).

### <a name="why-can-i-only-create-pbie-in-a-specific-region"></a>Por que só posso criar PBIE em uma região específica?

Você só pode criar as capacidades PBIE para sua região de locatário do PBI.

### <a name="how-can-i-find-what-is-my-pbi-tenant-region"></a>Como localizar qual é a minha região de locatário do PBI?

Você pode usar o portal do PBI para entender qual é a sua região de locatário do PBI.

[https://app.powerbi.com/](https://app.powerbi.com/) > ? > Sobre o Power BI

![Sobre o Power BI](media/embedded-faq/about-01.png)
![Região do locatário](media/embedded-faq/tenant-location-01.png)

### <a name="what-is-supported-with-the-cloud-solution-provider-csp-channel"></a>O que é compatível com o canal CSP (Provedor de Solução de Nuvem)?

* É possível criar o PBIE para seu locatário com o tipo de assinatura CSP
* A conta de parceiro pode ser conectada ao locatário do cliente e comprar o PBIE para o locatário do cliente, especificando o usuário do locatário do cliente como administrador de capacidade do Power BI

### <a name="why-do-i-get-an-unsupported-account-message"></a>Por que recebo uma mensagem de conta sem suporte?

O Power BI exige que você se inscreva com uma conta organizacional. Não é possível tentar se inscrever no Power BI usando uma MSA (conta Microsoft).

### <a name="can-i-use-apis-to-create--manage-azure-capacities"></a>Posso usar as APIs para criar e gerenciar as capacidades do Azure?

Sim, há cmdlets do Powershell e APIs do Azure Resource Manager que você pode usar para criar e gerenciar recursos de PBIE.

* APIs REST – https://docs.microsoft.com/rest/api/power-bi-embedded/
* Cmdlets do PowerShell – https://docs.microsoft.com/powershell/module/azurerm.powerbiembedded/

### <a name="what-is-the-pbi-embedded-dedicated-capacity-role-in-a-pbi-embedded-solution"></a>O que é a função de capacidade dedicada do PBI Incorporado em uma solução de PBI Incorporado?

Para [promover sua solução para produção](https://docs.microsoft.com/power-bi/developer/embedding-content#step-3-promote-your-solution-to-production), você precisa do conteúdo do Power BI (workspace do aplicativo que você está usando em seus aplicativos para atribuir a uma capacidade do Power BI Embedded (uma SKU).

### <a name="what-are-the-azure-regions-pbi-embedded-is-available"></a>Quais são as regiões do Azure que o PBI Incorporado está disponível?

[PAM](https://ecosystemmanager.azurewebsites.net/home) (EcoManager) – consulte o gerenciador de disponibilidade do produto

Regiões disponíveis (16 – nas mesmas regiões que o Power BI)

* EUA (6) – Leste dos EUA, Leste dos EUA 2, Centro-Norte dos EUA, Centro-Sul dos EUA, Oeste dos EUA, Oeste dos EUA 2
* Europa (2) – Europa Setentrional, Europa Ocidental
* Pacífico Asiático (2) – Sudeste Asiático, Ásia Oriental
* Brasil (1) – Sul do Brasil
* Japão (1) – Leste do Japão
* Austrália (1) – Sudeste da Austrália
* Índia (1) – Índia Ocidental
* Canadá (1) – Canadá Central
* Reino Unido (1) – Sul do Reino Unido

### <a name="what-is-the-authentication-model-for-power-bi-embedded"></a>Qual é o modelo de autenticação do Power BI Embedded?

O Power BI Embedded continuará a usar o Azure AD para autenticação do usuário mestre (um usuário licenciado designado do Power BI Pro), que autenticará o aplicativo no Power BI.

A autenticação e a autorização dos usuários do aplicativo serão implementadas pelo ISV, que poderá implementar uma autenticação própria para seus aplicativos.

Se você já tiver um locatário do Azure AD, será possível usar o diretório existente ou criar um novo locatário do Azure AD para a segurança do conteúdo do aplicativo inserido.

Para obter um token do AAD, você pode usar uma das bibliotecas de autenticação do Azure Active Directory – https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries. Bibliotecas de cliente estão disponíveis para várias plataformas.

### <a name="my-application-already-uses-aad-for-user-authentication-how-can-we-use-this-identity-when-authenticating-to-power-bi-in-an-user-owns-data-scenario"></a>Meu aplicativo já utiliza o AAD para autenticação do usuário. Como podemos usar essa identidade ao fazer a autenticação com o Power BI em um cenário "Usuário proprietário dos dados"?

É um fluxo padrão "em nome de" do OAuth (https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios#web-application-to-web-api)O aplicativo precisa ser configurado para exigir as permissões para o serviço do Power BI (com os escopos necessários) e, após ter um token de usuário para seu aplicativo, você simplesmente chama o AcquireTokenAsync da API ADAL usando o token de acesso do usuário e especifica a URL de recurso do Power BI como a ID de recurso. Veja a seguir um trecho de código que mostra como isso pode ser feito:

```csharp
var context = new AD.AuthenticationContext(authorityUrl);
var userAssertion = new AD.UserAssertion(userAccessToken);
var clientAssertion = new AD.ClientAssertionCertificate(MyAppId, MyAppCertificate)
var authenticationResult = await context.AcquireTokenAsync(resourceId, clientAssertion, userAssertion);
```

### <a name="how-is-power-bi-embedded-different-from-other-azure-services"></a>Qual a diferença entre o Power BI Embedded e os serviços do Azure?

O ISV/desenvolvedor deve ter uma conta do Power BI antes de comprar o Power BI Embedded no Azure. A região da implantação do Power BI Embedded é determinada pela conta do Power BI. Gerencie o recurso do Power BI Embedded no Azure para:

* Aumentar/reduzir
* Adicionar administradores de capacidade
* Pausar/retomar o serviço

Use o PowerBI.com para atribuir/cancelar a atribuição de workspaces à capacidade do Power BI Embedded.

### <a name="what-deploy-regions-are-supported"></a>Quais regiões de implantação são compatíveis?

Sudeste da Austrália, Sul do Brasil, Central do Canadá Central, Leste dos EUA 2, Índia Ocidental, Leste do Japão, Centro-Norte dos EUA, Europa Setentrional, Centro-Sul dos EUA, Sudeste Asiático, Sul do Reino Unido, Europa Ocidental, Oeste dos EUA e Oeste dos EUA 2.

### <a name="what-type-of-content-pack-data-can-be-embedded"></a>Que tipo de dados de pacote de conteúdo pode ser inserido?

**Dashboards** e **blocos** que são criados com base em conjuntos de dados de pacote de conteúdo *não podem* ser inseridos, porém **relatórios** criados com base em um conjunto de dados de pacote de conteúdo *podem* ser inseridos.

### <a name="what-is-the-difference-between-using-rls-vs-javascript-filters"></a>Qual é a diferença entre usar filtros RLS em vez de JavaScript?

Geralmente, há uma confusão sobre quando usar os filtros RLS em vez de JavaScript porque um método se trata de como controlar o que um usuário específico pode ver e o outro trata de como otimizar a exibição do usuário.

Para RLS, o desenvolvedor ISV controla a filtragem de dados como parte da criação do modelo e da geração de tokens inseridos. O usuário final vê apenas o que o ISV permitir. Neste caso, o usuário pode optar por ver menos do que o que está sendo filtrado, mas não conseguirá ignorar a configuração de RLS e ver mais do que o permitido.

Para filtragem do lado cliente (JavaScript ), o ISV pode decidir o que o usuário final vê na exibição inicial, mas não pode controlar as alterações que o usuário final pode aplicar à própria exibição. Mesmo que a filtragem de dados possa ocorrer no back-end, ela é acionada pelo código JavaScript do cliente e, portanto, pode ser alterada por um usuário final e não pode ser considerada segura.

Confira mais detalhes na referência [Filtros RLS vs JavaScript](embedded-row-level-security.md#using-rls-vs-javascript-filters).

### <a name="what-are-the-best-practices-to-improve-performance"></a>Quais são as práticas recomendadas para melhorar o desempenho?

[Desempenho do Power BI Embedded](embedded-performance-best-practices.md)

## <a name="licensing"></a>Licenças

### <a name="how-do-i-purchase-power-bi-embedded"></a>Como fazer para comprar o Power BI Embedded?

O Power BI Embedded está disponível por meio do Azure.

### <a name="what-happens-if-i-already-purchased-power-bi-premium-and-now-i-want-some-of-the-benefits-of-power-bi-embedded-in-azure"></a>O que acontece se já comprei o Power BI Premium e agora quero alguns dos benefícios do Power BI Embedded no Azure?

Os clientes continuarão a pagar pelas compras existentes do Power BI Premium até o término do prazo do contrato atual e, em seguida, poderão mudar as compras do Power BI Premium conforme necessário em tal momento.

### <a name="do-i-still-have-to-buy-power-bi-premium-to-get-access-to-power-bi-embedded"></a>Ainda preciso comprar o Power BI Premium para obter acesso ao Power BI Embedded?

Não, o Power BI Embedded inclui a capacidade baseada no Azure de que você precisa para implantar e distribuir sua solução aos clientes.

### <a name="whats-the-purchase-commitment-for-power-bi-embedded"></a>O que é a confirmação de compra para o Power BI Embedded?

Os clientes podem alterar o uso a cada hora. Não há nenhum compromisso mensal nem anual pelo serviço do Power BI Embedded.

### <a name="how-does-the-usage-of-power-bi-embedded-show-up-on-my-bill"></a>Como o uso do Power BI Embedded aparece na minha fatura?

O Power BI Embedded é cobrado em uma taxa por hora previsível com base nos tipos de nós implantados. Enquanto o recurso estiver ativo, você será cobrado mesmo se não houver uso. Para interromper a cobrança, é necessário pausar ativamente o recurso.

### <a name="who-needs-a-power-bi-pro-license-for-power-bi-embedded-and-why"></a>Quem precisa de uma licença do Power BI Pro para o Power BI Embedded e por quê?

A licença do Power BI Pro é necessária para analistas que precisam adicionar relatórios a um workspace do Power BI, para desenvolvedores que precisam usar as APIs REST e para administradores de locatários que precisam gerenciar o locatário e a capacidade do Power BI.

Uma vez que o Power BI Embedded permite o uso do portal do Power BI para gerenciar e validar o conteúdo inserido, a licença do Power BI Pro é necessária para autenticar o aplicativo no PowerBI.com para a obtenção do acesso aos relatórios nos repositórios corretos.

No entanto, para a [criação/edição de relatórios inseridos](https://github.com/Microsoft/PowerBI-JavaScript/wiki/Create-Report-in-Embed-View) dentro de seu próprio aplicativo, o usuário final não precisa ter uma licença Pro, pois ele não precisa ser um usuário do Power BI.

### <a name="can-i-get-started-for-free"></a>Posso começar gratuitamente?

Sim. Você pode usar os [créditos Azure](https://azure.microsoft.com/free/) para o Power BI Embedded.

### <a name="can-i-get-a-trial-experience-for-power-bi-embedded-in-azure"></a>Posso experimentar uma avaliação do Power BI Embedded no Azure?

Como o Power BI Embedded faz parte do Azure, é possível usar o serviço com o [crédito de US$ 200 recebido durante a inscrição no Azure](https://azure.microsoft.com/free/).

### <a name="is-power-bi-embedded-available-for-sovereign-clouds-us-government-germany-china"></a>O Power BI Embedded está disponível para nuvens soberanas (Governo dos EUA, Alemanha, China)?

O Power BI Embedded está disponível para algumas [nuvens soberanas](embed-sample-for-customers-sovereign-clouds.md). Ainda **NÃO** está disponível para a nuvem na China.

### <a name="is-power-bi-embedded-available-for-non-profits-and-educational"></a>O Power BI Embedded está disponível para entidades sem fins lucrativos e educacionais?

As entidades sem fins lucrativos e educacionais podem comprar o Azure. Não há nenhum preço especial para esses tipos de clientes no Azure.

## <a name="power-bi-workspace-collection"></a>Coleção de workspaces do Power BI

### <a name="what-is-power-bi-workspace-collection"></a>O que é a Coleção de workspaces do Power BI?

A **Coleção de workspaces do Power BI** (**Power BI Embedded** versão 1) é uma solução baseada no recurso de **Coleção de workspaces do Power BI** do Azure. Essa solução permite criar aplicativos do **Power BI Embedded** para seus clientes usando conteúdo do Power BI na solução **Coleção de workspaces do Power BI**, APIs dedicadas e chaves de coleção de workspaces para autenticar o aplicativo no Power BI.

### <a name="can-i-migrate-from-power-bi-workspace-collection-to-power-bi-embedded"></a>Posso migrar da Coleção de workspaces do Power BI para o Power BI Embedded?

1. Você pode usar a ferramenta de migração para clonar o conteúdo da **Coleção de workspaces do Power BI** no Power BI – https://docs.microsoft.com/power-bi/developer/migrate-from-powerbi-embedded#content-migration.

2. Comece com o POC do aplicativo **Power BI Embedded** que usa o conteúdo do Power BI.

3. Quando estiver pronto para a produção, compre uma capacidade dedicada do **Power BI Embedded** e atribua seu conteúdo do Power BI (workspace) a essa capacidade.

    > [!Note]
    > Você pode continuar usando a **Coleção de workspaces do Power BI** enquanto compila em paralelo com uma solução **Power BI Embedded**. Quando estiver pronto, você poderá mover o cliente para a nova solução **Power BI Embedded** e desativar a solução **Coleção de workspaces do Power BI**.

Para obter mais informações, confira [Como migrar o conteúdo da Coleção de workspaces do Power BI para o Power BI Embedded](https://docs.microsoft.com/power-bi/developer/migrate-from-powerbi-embedded)

### <a name="is-power-bi-workspace-collection-on-a-path-to-be-deprecated"></a>A Coleção de workspaces do Power BI está a caminho de ser preterida?

Sim, mas os clientes que já estão usando a solução **Coleção de workspaces do Power BI** podem continuar usando-a até que seja preterida. Os clientes também podem criar novas coleções de workspaces e qualquer aplicativo do **Power BI Embedded** que ainda usa a **Coleção de workspaces do Power BI**.

No entanto, isso também significa que novos recursos não serão adicionados a nenhuma solução da **Coleção de workspaces do Power BI** e que os clientes são incentivados a planejar sua migração para a nova solução **Power BI Embedded**.

### <a name="when-will-power-bi-workspace-collection-support-be-discontinued"></a>Quando o suporte para a Coleção de workspaces do Power BI será descontinuado?

Os clientes que já usam a solução **Coleções de workspace do Power BI** podem continuar usando-a até o final de junho de 2018 ou até o término do contrato de suporte.

### <a name="in-what-regions-can-pbi-workspace-collection-be-created"></a>Em quais regiões a Coleção de Workspaces do PBI pode ser criada?

As regiões disponíveis são Sudeste da Austrália, Sul do Brasil, Canadá Central, Leste dos EUA 2, Leste do Japão, Centro-Norte dos EUA, Europa Setentrional, Centro-Sul dos EUA, Sudeste Asiático, Sul do Reino Unido, Europa Ocidental, Índia Ocidental e Oeste dos EUA.

### <a name="why-should-i-migrate-from-pbi-workspace-collection-to-power-bi-embedded"></a>Por que migrar da Coleção de Workspaces do PBI para o Power BI Embedded?

Há novos recursos e funcionalidades que foram introduzidos na solução **Power BI Embedded** que você não pode fazer com a **Coleção de workspaces do Power BI**.

Alguns deles são:

* Todas as fontes de dados do PBI têm suporte, em contraste com as duas fontes de dados da **Coleção de workspaces do Power BI**. 
* Os novos recursos como P e R, atualizar, indicadores, inserção de painéis e blocos, menu personalizado etc. só têm suporte na solução **Power BI Embedded**.
* Modelo de cobrança por capacidade.

## <a name="embedding-setup-tool"></a>Ferramenta de configuração de inserção

### <a name="what-is-the-embedding-setup-tool"></a>O que é a ferramenta de configuração de inserção?

A [Ferramenta de configuração de inserção](https://aka.ms/embedsetup) permite iniciar rapidamente e baixar um aplicativo de exemplo para começar a inserção com o Power BI.

### <a name="which-solution-should-i-choose"></a>Qual solução devo escolher?

* A [inserção para clientes](embedding.md#embedding-for-your-customers) fornece a capacidade de inserir os dashboards e relatórios para usuários que não têm uma conta do Power BI. Execute a solução [Inserir para clientes](https://aka.ms/embedsetup/AppOwnsData).
* A [inserção para a organização](embedding.md#embedding-for-your-organization) permite que você estenda o serviço do Power BI. Execute a solução [Inserir para a organização](https://aka.ms/embedsetup/UserOwnsData).

### <a name="ive-downloaded-the-sample-app-which-solution-do-i-choose"></a>Baixei o aplicativo de exemplo. Qual solução devo escolher?

Se você estiver trabalhando com a experiência **Inserir para clientes**, salve e descompacte o arquivo *PowerBI-Developer-Samples.zip*. Em seguida, abra a pasta *PowerBI-Developer-Samples-master\App Owns Data* e execute o arquivo *PowerBIEmbedded_AppOwnsData.sln*.

Se você estiver trabalhando com a experiência **Inserir para a organização**, salve e descompacte o arquivo *PowerBI-Developer-Samples.zip*. Abra a pasta *PowerBI-Developer-Samples-master\User Owns Data\integrate-report-web-app* e execute o arquivo *pbi-saas-embed-report.sln*.

### <a name="how-can-i-edit-my-registered-application"></a>Como posso editar meu aplicativo registrado?

Você pode aprender a editar aplicativos registrados no AAD [aqui](https://docs.microsoft.com/azure/active-directory/develop/active-directory-integrating-applications#updating-an-application).

### <a name="how-can-i-edit-my-power-bi-user-profile-or-data"></a>Como editar meu perfil do usuário os dados no Power BI?

Você pode aprender a editar os dados do Power BI [aqui](https://docs.microsoft.com/power-bi/service-basic-concepts).

Para saber mais, veja [Solução de problemas de seu aplicativo inserido](embedded-troubleshoot.md).

Mais perguntas? [Experimente a Comunidade do Power BI](http://community.powerbi.com/)