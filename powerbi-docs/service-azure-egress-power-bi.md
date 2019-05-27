---
title: Saída do Power BI e do Azure
description: Entender os encargos de saída do Azure e Power BI com base no local do locatário e o Power BI Premium
author: davidiseminger
manager: kfile
ms.reviewer: ''
ms.service: powerbi
ms.subservice: powerbi-service
ms.topic: conceptual
ms.date: 05/08/2019
ms.author: davidi
LocalizationGroup: Data from databases
ms.openlocfilehash: 720ef2f059c3c87be84c3d8db98e89400c161ad0
ms.sourcegitcommit: 10a87c016f497dbeba32f94ed1f3688a70816fea
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2019
ms.locfileid: "65514399"
---
# <a name="power-bi-and-azure-egress"></a>Saída do Power BI e do Azure

Ao usar o Power BI com fontes de dados do Azure, você pode evitar encargos de saída do Azure verificando se o locatário do Power BI está na mesma região que suas fontes de dados do Azure.

Quando seu locatário do Power BI está implantado na mesma região do Azure ao implantar suas fontes de dados, você não incorrerá em encargos de saída para a atualização agendada e interações de DirectQuery. 

## <a name="determining-where-your-power-bi-tenant-is-located"></a>Determinar onde se encontra seu locatário do Power BI

Para descobrir onde seu locatário do Power BI está localizado, confira o artigo [onde meu locatário do Power BI está localizado](service-admin-where-is-my-tenant-located.md).

Para clientes do Power BI Premium Multi-Geo, se o locatário do Power BI não estiver no local ideal para algumas das suas fontes de dados do Azure, você poderá implantar o Power BI Premium Multi-Geo na região do Azure desejada e se beneficiar de ter o locatário do Power BI e as fonte de dados do Azure na mesma região do Azure.

## <a name="next-steps"></a>Próximas etapas

Para obter mais informações sobre o Power BI Premium ou Multi-Geo, observe os seguintes recursos:

* [O que é o Microsoft Power BI Premium?](service-premium-what-is.md)
* [Como comprar o Power BI Premium](service-admin-premium-purchase.md)
* [Compatibilidade do Multi-Geo com o Power BI Premium (versão prévia)](service-admin-premium-multi-geo.md)
* [Onde está localizado meu locatário do Power BI?](service-admin-where-is-my-tenant-located.md)
* [Perguntas Frequentes do Power BI Premium](service-premium-faq.md)


