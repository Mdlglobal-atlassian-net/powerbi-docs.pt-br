---
title: Solucionando problemas de erros de bloco
description: Erros comuns que podem ser encontrados quando um bloco tenta ser atualizado no Power BI
author: davidiseminger
manager: kfile
ms.reviewer: ''
ms.custom: seodec18
ms.service: powerbi
ms.subservice: powerbi-service
ms.topic: conceptual
ms.date: 12/06/2018
ms.author: davidi
LocalizationGroup: Troubleshooting
ms.openlocfilehash: bfb6178908a9d6a4bcfe81f8d3d9771ac5b12b9d
ms.sourcegitcommit: 88ac51106ec7d0ead8c2a1550a11afae0d502bb9
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/12/2019
ms.locfileid: "56086622"
---
# <a name="troubleshooting-tile-errors"></a>Solucionando problemas de erros de bloco
Veja abaixo os erros comuns que podem ser encontrados com blocos e uma explicação.

> [!NOTE]
> Se você encontrar um erro que não esteja listado abaixo, e que esteja causando problemas, solicite ajuda no [site da comunidade](http://community.powerbi.com/) ou crie um [tíquete de suporte](https://powerbi.microsoft.com/support/).
> 
> 

## <a name="errors"></a>Erros
**O Power BI encontrou um erro inesperado ao carregar o modelo. Tente novamente mais tarde.**
ou **Não foi possível recuperar o modelo de dados. Entre em contato com o proprietário do painel para ter certeza de que as fontes e o modelo de dados existem e estão acessíveis.**

Não conseguimos acessar os dados, porque a fonte de dados não estava acessível. Esse problema pode ocorrer se a fonte de dados é removida, renomeada, movida, fica offline ou se as permissões são alteradas. Verifique se a fonte ainda está no local para o qual estamos apontando e se você ainda tem permissão para acessá-la. Se esse não for o problema, a fonte pode estar lenta. Tente novamente mais tarde em um horário em que a carga na fonte é menor. Se for uma origem local, o proprietário da fonte de dados poderá conseguir fornecer mais informações.

**Você não tem permissão para exibir este bloco ou abra a pasta de trabalho.**

Contate o proprietário do dashboard para verificar se o modelo e as fontes de dados existem e se estão acessíveis para sua conta.

**Os visuais personalizados foram desabilitados pelo administrador.**

O administrador do Power BI desabilitou o uso de visuais personalizados para sua organização ou seu grupo de segurança. Você não poderá usar visuais personalizados no [Microsoft Marketplace](https://appsource.microsoft.com/en-us/marketplace/apps?page=1&product=power-bi-visuals) nem importar visuais particulares por meio de um arquivo. Você só poderá usar o conjunto pré-empacotado de visuais.


**As formas de dados devem conter ao menos um grupo ou cálculo que produza dados. Entre em contato com o proprietário do painel.**

Não temos nenhum dado para exibir, pois a consulta está vazia. Tente adicionar alguns campos na lista de campos ao visual e fixá-lo novamente.

**Não é possível exibir os dados, porque o Power BI não pode determinar o relacionamento entre dois ou mais campos.**

Você está tentando usar dois ou mais campos de tabelas que não estão relacionadas. Você precisa remover os campos não relacionados do visual e, em seguida, criar um relacionamento entre as tabelas. Depois de fazer essa alteração, você poderá adicionar os campos novamente ao visual. Isso pode ser feito no Power BI Desktop ou no Power Pivot para Excel. [Saiba mais](desktop-create-and-manage-relationships.md)

**Os grupos no eixo primário e no eixo secundário se sobrepõem. Os grupos no eixo primário não podem ter as mesmas chaves que os grupos no eixo secundário.**

Geralmente, esse é um problema temporário. Isso geralmente acontece quando você está movendo grupos de linhas para colunas. Nesse caso, o erro deverá desaparecer quando você terminar de mover todos os grupos. Se você ainda vir a mensagem, tente alternar os campos entre as linhas e colunas ou a legenda de eixo ou remover campos do visual.  

**Este visual excedeu os recursos disponíveis. Tente filtrar para diminuir a quantidade de dados exibidos.**

O visual tentou consultar um número excessivo de dados para que possamos concluir o resultado com os recursos disponíveis. Tente filtrar o visual para reduzir a quantidade de dados no resultado.

**Não conseguimos identificar os seguintes campos: {0}. Atualize o visual com campos existentes no conjunto de dados.**

O campo provavelmente foi excluído ou renomeado. É possível remover o campo quebrado do visual, adicionar outro campo e fixá-lo novamente.

**Não foi possível recuperar os dados deste visual. Tente novamente mais tarde.**

Isso geralmente é um problema temporário. Se você tentar novamente mais tarde e ainda receber essa mensagem, contate o suporte.

## <a name="contact-support"></a>Contatar o suporte
Caso ainda esteja tendo algum problema, [contate o suporte](https://support.powerbi.com) para investigá-lo mais detalhadamente.

## <a name="next-steps"></a>Próximas etapas
[Solução de problemas do gateway de dados local](service-gateway-onprem-tshoot.md)  
[Solução de problemas do Power BI Personal Gateway](service-admin-troubleshooting-power-bi-personal-gateway.md)  
Mais perguntas? [Experimente a Comunidade do Power BI](http://community.powerbi.com/)

