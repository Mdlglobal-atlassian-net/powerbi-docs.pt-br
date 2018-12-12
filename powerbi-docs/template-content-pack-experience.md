---
title: Experiências de pacote de conteúdo de modelo no Power BI
description: Experiências do Pacote de Conteúdo de Modelo
author: maggiesMSFT
manager: kfile
ms.reviewer: ''
ms.service: powerbi
ms.component: powerbi-service
ms.topic: conceptual
ms.date: 10/09/2017
ms.author: maggies
ms.openlocfilehash: 23a8875479197f1d200a9f086fcfd27d483faf40
ms.sourcegitcommit: b03912343a5a214c6bb972aaa6aa051c2a5f4332
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/05/2018
ms.locfileid: "52900211"
---
# <a name="template-content-pack-experiences-in-power-bi"></a>Experiências de pacote de conteúdo de modelo no Power BI
Esta seção destaca uma experiência típica de um usuário se conectando a um [pacote de conteúdo](service-connect-to-services.md) de ISV.

Tenha a experiência de conexão você mesmo conectando-se a um pacote de conteúdo lançado em https://app.powerbi.com/getdata/services (como o [pacote de conteúdo do GitHub](https://app.powerbi.com/getdata/services/github) descrito abaixo).

## <a name="connect"></a>Conectar
Para começar, o usuário navega pela galeria de pacotes de conteúdo e seleciona um pacote de conteúdo para se conectar. A entrada do pacote de conteúdo fornece um nome, um ícone e um texto descritivo que fornece mais informações para o usuário.

![conectar-se](media/template-content-pack-experience/github_data.png)

![conectar-se](media/template-content-pack-experience/github_connect.png)

## <a name="parameters"></a>Parâmetros
Após selecionar, o usuário será solicitado a fornecer parâmetros (se necessários). A caixa de diálogo de parâmetros é fornecida declarativamente pelo autor durante a criação do pacote de conteúdo.

Atualmente, a interface do usuário dos parâmetros é bem básica – não é possível enumerar as listas suspensas e a validação de entrada de dados é restrita a regex.

![parâmetros](media/template-content-pack-experience/github_params.png)

## <a name="credentials"></a>Credenciais
Depois dos parâmetros, o usuário deverá fazer logon.  Se a fonte der suporte a vários tipos de autenticação, o usuário escolherá a opção apropriada. Se a fonte exigir OAuth, a UI de logon do serviço será exibida quando o usuário pressionar Entrar.  Caso contrário, o usuário pode inserir suas credenciais na caixa de diálogo fornecida.

![Credenciais](media/template-content-pack-experience/github_login.png)

![conectar-se](media/template-content-pack-experience/github_creds2.png)

## <a name="instantiation"></a>Instanciação
Quando o logon for bem-sucedido, os artefatos incluídos no pacote de conteúdo - modelo, relatórios e painel - aparecerão na barra de navegação.  Esses artefatos são adicionados à conta de cada usuário.  Os dados são carregados de forma assíncrona para preencher o conjunto de dados (modelo).  O usuário, então, é capaz de consumir o painel, os relatórios e o modelo.

Por padrão, uma agenda de atualização diária é configurada para o usuário, o que avaliará novamente as consultas no modelo.  As credenciais fornecidas ao usuário devem permitir que eles atualizem os dados sem estarem presentes.

![Instanciação](media/template-content-pack-experience/github_dashboard.png)

## <a name="exploration-and-monitoring"></a>Exploração e monitoramento
Após o pacote de conteúdo ser serializado na conta do usuário, ele pode explorar e monitorar as informações/dados.

Normalmente, isso inclui:

* Exibir e personalizar o painel.
* Exibir e personalizar o relatório.
* Usar linguagem natural para fazer perguntas aos dados
* Usar a tela de exploração para explorar os dados no modelo de dados

É necessário levar em consideração o fornecimento de modelagem de linguagem natural (sinônimos) e um esquema de modelo compreensível para permitir melhores experiências de exploração.

