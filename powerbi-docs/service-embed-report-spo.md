---
title: Inserir com Web Part de Relatório no SharePoint Online
description: Com a nova Web Part de Relatório do Power BI para o SharePoint Online, você pode facilmente inserir relatórios interativos do Power BI às páginas do SharePoint Online.
author: markingmyname
ms.author: maghan
manager: kfile
ms.reviewer: ''
featuredvideoid: ''
ms.service: powerbi
ms.component: powerbi-service
ms.topic: conceptual
LocalizationGroup: Share your work
ms.date: 10/20/2018
ms.openlocfilehash: e336323863dfacc8c74f2dc1f721231d58d03834
ms.sourcegitcommit: 60fb46b61ac73806987847d9c606993c0e14fb30
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/25/2018
ms.locfileid: "50100762"
---
# <a name="embed-with-report-web-part-in-sharepoint-online"></a>Inserir com Web Part de Relatório no SharePoint Online

Com a nova Web Part de Relatório do Power BI para o SharePoint Online, você pode facilmente inserir relatórios interativos do Power BI às páginas do SharePoint Online.

Ao usar a nova opção **Inserir ao SharePoint Online**, os relatórios incorporados são totalmente protegidos para que você possa facilmente criar portais internos seguros.

## <a name="requirements"></a>Requisitos

Há alguns requisitos para que os relatórios da opção **Inserir ao SharePoint Online** funcionem.

* Você precisa de uma licença do Power BI Pro ou de uma [capacidade do Power BI Premium (EM ou SKU P)](service-premium.md#premium-capacity-nodes) com uma licença do Power BI.
* A web part do Power BI para o SharePoint Online requer [Páginas Modernas](https://support.office.com/article/Allow-or-prevent-creation-of-modern-site-pages-by-end-users-c41d9cc8-c5c0-46b4-8b87-ea66abc6e63b).

## <a name="embed-your-report"></a>Insira seu relatório

Para inserir seu relatório no SharePoint Online, primeiro você precisa obter a URL do relatório e, em seguida, usá-la com a nova web part do Power BI no SharePoint Online.

### <a name="get-a-url-to-your-report"></a>Obter a URL do relatório

1. Exibir o relatório no serviço do Power BI.

2. Selecionar o item de menu **Arquivo**.

3. Selecione **Inserir no SharePoint Online**.

    ![Menu Arquivo](media/service-embed-report-spo/powerbi-file-menu.png)

4. Copiar a URL da caixa de diálogo.

    ![Inserir link](media/service-embed-report-spo/powerbi-embed-link-sharepoint.png)

### <a name="add-the-power-bi-report-to-a-sharepoint-online-page"></a>Adicionar o relatório do Power BI a uma página do SharePoint Online

1. Abra a página desejada no SharePoint Online e selecione **Editar**.

    ![Página de edições do SP](media/service-embed-report-spo/powerbi-sharepoint-edit-page.png)

    Ou crie uma nova página de site selecionando **+ novo** dentro do SharePoint Online.

    ![Nova página do SP](media/service-embed-report-spo/powerbi-sharepoint-new-page.png)

2. Selecione **+** e selecione a web part do **Power BI**.

    ![Nova web part do SP](media/service-embed-report-spo/powerbi-sharepoint-new-web-part.png)

3. Selecione **Adicionar relatório**.

    ![Novo relatório do SP](media/service-embed-report-spo/powerbi-sharepoint-new-report.png)

4. Cole a URL do relatório no painel de propriedade. Esta URL do relatório é a URL que você copiou das etapas acima. O relatório é carregado automaticamente.

    ![Novas propriedades da web part do SP](media/service-embed-report-spo/powerbi-sharepoint-new-web-part-properties.png)

5. Selecione **Publicar** para tornar a alteração visível para os usuários do SharePoint Online.

    ![Relatório do SP carregado](media/service-embed-report-spo/powerbi-sharepoint-report-loaded.png)

## <a name="granting-access-to-reports"></a>Conceder acesso aos relatórios

Incorporar um relatório ao SharePoint Online automaticamente não dá aos usuários permissão para exibir o relatório. As permissões para exibir o relatório são definidas dentro do serviço do Power BI.

> [!IMPORTANT]
> Certifique-se de examinar quem pode ver o relatório dentro do serviço do Power BI e de conceder acesso aos que não aparecem na lista.

Há duas maneiras de conceder acesso ao relatório dentro do serviço do Power BI. Se você estiver usando um grupo do Office 365 para criar seu site de equipe do SharePoint Online, liste o usuário como membro do **workspace do aplicativo no serviço do Power BI** e da **página do SharePoint**. Isso garante que os usuários possam exibir o conteúdo desse grupo. Para obter mais informações, consulte [Criar e distribuir um aplicativo no Power BI](service-create-distribute-apps.md).

Como alternativa, você pode compartilhar um relatório diretamente com os usuários, incorporando o relatório a um aplicativo. O aplicativo deve estar pré-instalado para que o relatório seja incorporado. Você pode configurar o aplicativo para ser pré-instalado usando o recurso **Instalar aplicativo automaticamente**.

   ![Instalar o aplicativo automaticamente](media/service-embed-report-spo/install-app-automatically.png)

> [!NOTE]
> **O usuário precisa acessar a página do SharePoint e o relatório para ver o relatório na página do SharePoint.**

## <a name="multi-factor-authentication"></a>Autenticação multifator

Se o ambiente do Power BI exigir que você entre usando a autenticação multifator, talvez será necessário entrar com um dispositivo de segurança para verificar sua identidade. Isso ocorre quando você não entra no SharePoint Online usando a autenticação multifator, mas o ambiente do Power BI requer uma conta validada por um dispositivo de segurança.

> [!NOTE]
> O Azure Active Directory 2.0 ainda não dá suporte para autenticação multifator. Os usuários recebem uma mensagem indicando *erro*. Se o usuário entrar novamente no SharePoint Online usando o dispositivo de segurança, o relatório poderá ser exibido.

## <a name="web-part-settings"></a>Configurações de Web Part

Abaixo, temos uma descrição das configurações que podem ser ajustadas para a web part do Power BI para o SharePoint Online.

![Propriedades da web part do SP](media/service-embed-report-spo/powerbi-sharepoint-web-part-properties.png)

| Propriedade | Descrição |
| --- | --- |
| Nome da página |Define a página padrão que é exibida pela web part. Selecione um valor na lista suspensa. Se nenhuma página for exibida, o relatório terá uma página ou a URL que você colou conterá um nome de página. Remover a seção de relatório da URL para selecionar uma página específica. |
| Exibição |Opção para ajustar como o relatório é ajustado dentro da página do SharePoint Online. |
| Exibir o Painel de Navegação |Exibe ou oculta o painel de navegação da página. |
| Exibir Painel de Filtro |Exibe ou oculta o painel de filtro. |

## <a name="reports-that-do-not-load"></a>Relatórios que não são carregados

O relatório pode não ser carregado dentro da web part do Power BI e a seguinte mensagem pode ser exibida.

*Este conteúdo não está disponível.*

![Mensagem Relatório não encontrado](media/service-embed-report-spo/powerbi-sharepoint-report-not-found.png)

Há duas razões comuns para essa mensagem.

1. Você não tem acesso a este relatório.
2. O relatório foi excluído.

Contate o proprietário da página do SharePoint Online para ajudá-lo a resolver o problema.

## <a name="licensing"></a>Licenças

Os usuários que exibem um relatório no SharePoint precisam de uma **licença do Power BI Pro** ou o conteúdo precisa estar em um espaço de trabalho que esteja em uma capacidade do **[Power BI Premium (SKU EM ou P)](service-admin-premium-purchase.md)**.

## <a name="known-issues-and-limitations"></a>Limitações e problemas conhecidos

* Erro: "Ocorreu um erro, tente sair e entrar e, em seguida, visite esta página novamente. ID de correlação: status de resposta HTTP indefinido: 400, código 10001 de erro servidor, mensagem: token de atualização ausente"
  
  Se você receber esse erro, tente uma das etapas de solução de problemas abaixo.
  
  1. Saia do SharePoint e entre novamente. Certifique-se de fechar todas as janelas do navegador antes de entrar novamente.

  2. Se sua conta de usuário exige a MFA (autenticação multifator), entre no SharePoint usando o dispositivo de autenticação multifator (aplicativo de telefone, cartão inteligente, etc.)
  
  3. Contas de Usuários convidados B2B do Azure não são compatíveis. Os usuários veem o logotipo do Power BI que mostra a parte que está sendo carregada, mas o relatório não é mostrado.

* O Power BI não dá suporte aos mesmos idiomas localizados que o SharePoint Online. Como resultado, você não verá a localização correta no relatório inserido.

* Você pode encontrar problemas se usar o Internet Explorer 10. Você pode examinar o [suporte dos navegadores para o Power BI](consumer/end-user-browsers.md) e para o [Office 365](https://products.office.com/office-system-requirements#Browsers-section).

* A web part do Power BI não está disponível em [nuvens soberanas](https://powerbi.microsoft.com/en-us/clouds/).

* O servidor clássico do SharePoint não é compatível com essa web part.

* [Filtros de URL](service-url-filters.md) não são compatíveis com a Web part do SPO.

## <a name="next-steps"></a>Próximas etapas

[Permitir ou impedir a criação de páginas de sites modernas pelos usuários finais](https://support.office.com/article/Allow-or-prevent-creation-of-modern-site-pages-by-end-users-c41d9cc8-c5c0-46b4-8b87-ea66abc6e63b)  
[Criar e distribuir um aplicativo no Power BI](service-create-distribute-apps.md)  
[Compartilhar um painel com seus colegas e com outras pessoas](service-share-dashboards.md)  
[O que é o Power BI Premium?](service-premium.md)  

Mais perguntas? [Experimente perguntar à Comunidade do Power BI](http://community.powerbi.com/)