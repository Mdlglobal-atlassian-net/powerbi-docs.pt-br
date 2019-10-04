---
title: Filtrar relatório por localização geográfica em um aplicativo móvel do Power BI
description: Saiba como você pode filtrar um relatório por localização geográfica nos aplicativos móveis do Power BI da Microsoft se o proprietário do relatório definir marcações geográficas.
author: mshenhav
manager: kfile
ms.service: powerbi
ms.subservice: powerbi-mobile
ms.topic: conceptual
ms.date: 09/25/2019
ms.author: mshenhav
ms.openlocfilehash: 9a4950a1d52451764c3c62413bf4ecbd036f06c8
ms.sourcegitcommit: 57e45f291714ac99390996a163436fa1f76db427
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "71305766"
---
# <a name="filter-a-report-by-geographic-location-in-the-power-bi-mobile-apps"></a>Filtrar um relatório por localização geográfica nos aplicativos móveis do Power BI
Aplica-se a:

| ![iPhone](./media/mobile-apps-geographic-filtering/iphone-logo-50-px.png) | ![iPad](./media/mobile-apps-geographic-filtering/ipad-logo-50-px.png) | ![Telefone Android](./media/mobile-apps-geographic-filtering/android-phone-logo-50-px.png) | ![Tablet Android](./media/mobile-apps-geographic-filtering/win-10-logo-50-px.png) |
|:--- |:--- |:--- |:--- |
| iPhones |iPads |Telefones Android |Telefones Windows 10 |

Ao examinar um relatório do Power BI em seu dispositivo móvel, você vê um pequeno ícone de tachinha no canto superior direito? Nesse caso, você pode filtrar o relatório com base em sua localização geográfica.

> [!NOTE]
> Só será possível filtrar por localização se os nomes geográficos no relatório estiverem em inglês; por exemplo, “New York City” ou “Germany”. Tablets e PCs com Windows 10 não oferecem suporte a filtragem geográfica, mas celulares com Windows 10 fazem.
> 
> 

## <a name="filter-your-report-by-your-geographic-location"></a>Filtrar o relatório por localização geográfica
1. Abra um relatório no aplicativo móvel do Power BI em seu dispositivo móvel.
2. Se o relatório tiver dados geográficos, você verá uma mensagem pedindo para permitir que o Power BI acesse sua localização. Clique em **Permitir** e, em seguida, toque em **Permitir** novamente.
3. Toque na tachinha ![Ícone de tachinha](./media/mobile-apps-geographic-filtering/power-bi-mobile-geo-icon.png). Você pode filtrar por cidade, por estado/província ou por país/região, dependendo dos dados no relatório. O filtro lista apenas as opções que correspondem à sua localização atual.
   
    ![Filtro de tachinha](./media/mobile-apps-geographic-filtering/power-bi-mobile-geo-map-set-filter.png)

## <a name="why-dont-i-see-location-tags-on-a-report"></a>Por que não vejo marcações de localização em um relatório?
Todas as três condições abaixo precisam ser verdadeiras para que seja possível ver as marcações de localização. 

* A pessoa que criou o relatório no Power BI Desktop precisa ter [categorizado os dados geográficos](../../desktop-mobile-geofiltering.md) em pelo menos uma coluna, como cidade, estado ou país/região.
* Você está em um dos locais que contém dados nessa coluna.
* Você está usando um desses dispositivos móveis:
  * iOS (iPad, iPhone, iPod).
  * Telefone Android.
  * Celular com Windows 10 (outros dispositivos com Windows 10, como PCs e tablets que não dão suporte para filtragem geográfica).

Leia mais sobre a [configuração da filtragem geográfica](../../desktop-mobile-geofiltering.md) no Power BI Desktop.

### <a name="next-steps"></a>Próximas etapas
* [Conectar-se a dados do Power BI do mundo real](mobile-apps-data-in-real-world-context.md) com os aplicativos móveis
* [Categorização de dados no Power BI Desktop](../../desktop-data-categorization.md) 
* Dúvidas? [Experimente perguntar à Comunidade do Power BI](http://community.powerbi.com/)

