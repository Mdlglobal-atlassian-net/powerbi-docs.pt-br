---
title: Conectar-se ao Acumatica com o Power BI
description: Acumatica para o Power BI
author: SarinaJoan
manager: kfile
ms.reviewer: maggiesMSFT
ms.service: powerbi
ms.subservice: powerbi-template-apps
ms.topic: conceptual
ms.date: 08/29/2019
ms.author: sarinas
LocalizationGroup: Connect to services
ms.openlocfilehash: d2ee7a338f34e4c29fdbefae6518bede9e94badb
ms.sourcegitcommit: b53a6f5575f5f8bc443ecdca9c72525ce123518f
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/30/2019
ms.locfileid: "70186151"
---
# <a name="connect-to-acumatica-with-power-bi"></a>Conectar-se ao Acumatica com o Power BI
O pacote de conteúdo do Acumatica para o BI Power permite que você obtenha informações rapidamente sobre os dados de sua oportunidade. O Power BI recupera seus dados, incluindo oportunidades, contas e clientes, e cria um painel padrão e relatórios relacionados com base nesses dados.

[!INCLUDE [include-short-name](./includes/service-deprecate-content-packs.md)]

Conecte-se ao [pacote de conteúdo do Acumatica](https://app.powerbi.com/getdata/services/acumatica) ou leia mais sobre a [Integração do Acumatica](https://powerbi.microsoft.com/integrations/acumatica) com o Power BI.

>[!NOTE]
>Esse pacote de conteúdo exige o Acumatica v5.2 ou superior.

## <a name="how-to-connect"></a>Como se conectar
1. Selecione **Obter Dados** na parte inferior do painel de navegação esquerdo.
   
   ![](media/service-connect-to-acumatica/getdata3.png)
2. Na caixa **Serviços** , selecione **Obter**.
   
   ![](media/service-connect-to-acumatica/getdata2.png)
3. Selecione **Acumatica** \> **Obter**.
   
   ![](media/service-connect-to-acumatica/acumatica.png)
4. Insira o ponto de extremidade OData do Acumatica. Um ponto de extremidade OData permite que um sistema externo solicite dados do Acumatica. O ponto de extremidade OData do Acumatica é formatado da seguinte maneira e deve usar HTTPS:
   
     `https://[sitedomain]/odata/[companyname]`
   
   O Nome da Empresa só é necessário se você tiver uma implantação de várias empresas. Mais informações sobre como encontrar esse parâmetro em sua conta do Acumatica estão incluídas abaixo.
   
   ![](media/service-connect-to-acumatica/parameters.png)
5. Como o Método de Autenticação, selecione **Básico**. Digite seu nome de usuário e a senha de sua conta do Acumatica e clique em **Entrar**.
   
    ![](media/service-connect-to-acumatica/creds2.png)
6. Após o Power BI importar os dados, você verá novos elementos (painel, relatório e conjunto de dados) no painel de navegação esquerdo. Os novos itens são marcados com um asterisco amarelo \* que desaparece depois de selecionado. A escolha do dashboard mostrará um layout semelhante ao mostrado abaixo:
   
    ![](media/service-connect-to-acumatica/dashboard.png)

**E agora?**

* Tente [fazer uma pergunta na caixa de P e R](consumer/end-user-q-and-a.md) na parte superior do dashboard
* [Altere os blocos](service-dashboard-edit-tile.md) no dashboard.
* [Selecione um bloco](consumer/end-user-tiles.md) para abrir o relatório subjacente.
* Enquanto seu conjunto de dados será agendado para ser atualizado diariamente, você pode alterar o agendamento de atualização ou tentar atualizá-lo sob demanda usando **Atualizar Agora**

## <a name="system-requirements"></a>Requisitos de sistema
Este pacote de conteúdo exige o Acumatica v5.2 ou superior; confirme a versão com o administrador do Acumatica.

## <a name="finding-parameters"></a>Localizando parâmetros
**Ponto de extremidade OData do Acumatica**

O ponto de extremidade OData do Acumatica é formatado da seguinte maneira e deve usar HTTPS:

    https://[sitedomain]/odata/[companyname]

O Domínio do Site do Aplicativo pode ser encontrado na barra de endereços do navegador depois de entrar no Acumatica. No exemplo a seguir, o domínio do site é `https://pbi.acumatica.com`, de modo que o ponto de extremidade OData a se fornecer seria `https://pbi.acumatica.com/odata`.

 ![](media/service-connect-to-acumatica/url.png)

O Nome da Empresa só é necessário se você tiver uma implantação de várias empresas. Você pode encontrar essas informações na página de conexão do Acumatica.

![](media/service-connect-to-acumatica/signin2.png)

## <a name="troubleshooting"></a>Solução de problemas
Se você não conseguir fazer logon, verifique se o ponto de extremidade OData do Acumatica fornecido está formatado corretamente.

    https://<application site domain>/odata/<company name>

Se tiver problemas para se conectar, confirme com o administrador sua versão do Acumatica. Este pacote de conteúdo requer a versão 5.2 ou posterior.

## <a name="next-steps"></a>Próximas etapas
[Introdução ao Power BI](service-get-started.md)

[Obter dados no Power BI](service-get-data.md)

