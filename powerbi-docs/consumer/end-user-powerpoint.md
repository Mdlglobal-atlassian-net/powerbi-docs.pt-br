---
title: Exportar relatórios do Power BI para o PowerPoint
description: Saiba como exportar um relatório do Power BI para o PowerPoint.
author: mihart
manager: kvivek
ms.custom: seodec18
ms.reviewer: ''
ms.service: powerbi
ms.subservice: powerbi-consumer
ms.topic: conceptual
ms.date: 02/14/2019
ms.author: mihart
LocalizationGroup: Share your work
ms.openlocfilehash: 3563c19630d481f1d3601e314ee13e1aef5c597d
ms.sourcegitcommit: a054782370dec56d49bb205ee10b7e2018f22693
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/22/2019
ms.locfileid: "56661803"
---
# <a name="export-reports-from-power-bi-to-powerpoint"></a>Exportar relatórios do Power BI para o PowerPoint
Com o Power BI, você pode publicar seu relatório no **Microsoft PowerPoint** e criar facilmente um conjunto de slides com base em seu relatório do Power BI. Quando você **exporta para o PowerPoint**, ocorre o seguinte:

* Cada página no relatório do Power BI se torna um slide individual no PowerPoint
* Cada página no relatório do Power BI é exportada como uma única imagem de alta resolução no PowerPoint <!-- * The filters and slicers settings that you added to the report are preserved. -->
* É criado um link no PowerPoint que é vinculado ao relatório do Power BI 

Obter o **relatório do Power BI** exportado no **PowerPoint** é rápido. Basta seguir as etapas descritas na próxima seção.

## <a name="how-to-export-your-power-bi-report-to-powerpoint"></a>Como exportar um relatório do Power BI para o PowerPoint
No serviço do Power BI, selecione um relatório para exibi-lo na tela. Você também pode selecionar um relatório na **Página Inicial**, **Aplicativos** ou em qualquer outra seção no painel esquerdo.

![Seleção de Arquivo na barra de menus e seta apontando para Exportar para o PowerPoint](media/end-user-powerpoint/power-bi-publish.png)

Quando o relatório que você deseja exportar para o PowerPoint for exibido na tela, selecione **Arquivo > Exportar para o PowerPoint** na barra de menus do serviço do Power BI.

![Aproximação da barra de navegação esquerda com o Meu Espaço de Trabalho selecionado e o menu suspenso Arquivo selecionado](media/end-user-powerpoint/powerbi_to_powerpoint_1.png)
   
Um pop-up será exibido, em que você tem a opção de selecionar a **Exibição atual** ou a **Exibição padrão**.  A **Exibição atual** exporta o relatório no estado atual, que inclui as alterações ativas feitas nos valores de segmentação e filtro.  A maioria dos usuários seleciona essa opção.  Alternativamente, a seleção de **Exibição padrão** exporta o relatório em seu estado original (como o autor o compartilhou) e não reflete as alterações feitas no estado original.
    
Além disso, há uma caixa de seleção para marcar se você deseja ou não exportar as guias ocultas de um relatório.  Basta marcar essa caixa se desejar exportar somente as guias de relatório visíveis para você no navegador.  Se preferir obter todas as guias ocultas como parte da exportação, deixe-a desmarcada.  Se a caixa de seleção estiver esmaecida, não haverá guias ocultas no relatório.  Depois de fazer as seleções, clique em **Exportar** para continuar.

Você verá uma faixa de notificação no canto superior direito da janela do navegador de serviço do Power BI de que o relatório está sendo exportado para o PowerPoint. Isso pode levar alguns minutos e você pode continuar a trabalhar no Power BI enquanto o relatório está sendo exportado.

![notificação de exportação para o PowerPoint em andamento](media/end-user-powerpoint/powerbi_to_powerpoint_2.png)

Depois de concluído, o banner de notificação muda para informá-lo de que o serviço do Power BI terminou o processo de exportação.

![Exibição da mensagem de êxito](media/end-user-powerpoint/powerbi_to_powerpoint_3.png)

O arquivo estará disponível quando o navegador exibir os arquivos baixados. Na imagem a seguir, ele é mostrado como uma faixa de download na parte inferior da janela do navegador.

![seta apontando para a notificação do navegador na parte inferior da tela](media/end-user-powerpoint/powerbi_to_powerpoint_4.png)

E isso é tudo para ele. Você pode baixá-lo, abri-lo com o PowerPoint e, em seguida, modificá-lo ou aprimorá-lo exatamente como faria com qualquer outro material do PowerPoint.

## <a name="checking-out-your-exported-powerpoint-file"></a>Verificando o arquivo do PowerPoint exportado
Quando você abre o arquivo do PowerPoint que o Power BI exportou, encontra alguns elementos interessantes e úteis. Dê uma olhada na imagem a seguir e veja os elementos numerados abaixo dela que descrevem alguns desses recursos interessantes.

![O PowerPoint abre](media/end-user-powerpoint/powerbi_to_powerpoint_5.png)

1. A primeira página do conjunto de slides inclui o nome do relatório e um link para que você possa **Exibir no Power BI** o relatório no qual o conjunto de slides se baseia.
2. Você também obtém algumas informações úteis sobre o relatório, incluindo a *última atualização dos dados* em que o relatório exportado é baseado e a hora e data do *download*, que é a hora e a data em que o relatório do Power BI foi exportado para um arquivo PowerPoint.
3. Cada página do relatório é um slide separado, conforme mostrado no painel de navegação esquerdo. 
4. O relatório publicado é renderizado no idioma de acordo com as configurações do Power BI ou pela configuração de localidade do seu navegador. Para ver ou definir sua preferência de idioma, selecione o ![ícone de engrenagem](media/end-user-powerpoint/power-bi-settings-icon.png) **> Configurações > Geral > Idioma**. Para obter informações sobre localidade, confira [Idiomas com suporte e países/regiões do Power BI](../supported-languages-countries-regions.md).
5. A apresentação do PowerPoint inclui um slide de rosto com a hora de exportação no fuso horário correto.

Quando você entrar em um slide individual, perceberá que cada página de relatório é uma imagem independente.

>[!NOTE]
> Ter um visual para cada página do relatório é um novo comportamento. O comportamento anterior, que fornecia uma imagem independente para cada visual, não está mais implementado. 
 

![Imagem que mostra cada elemento visual como uma imagem separada](media/end-user-powerpoint/powerbi_to_powerpoint_6.png)

O que fazer com seu material do PowerPoint daí em diante, ou com qualquer uma das imagens em alta resolução, cabe a você!

## <a name="limitations"></a>Limitações
Há algumas considerações e limitações para ter em mente ao trabalhar com o recurso **Exportar para o PowerPoint**.

* No momento, não há suporte para **visuais do R**. Esses visuais são exportados como uma imagem em branco para o PowerPoint com uma mensagem de erro que afirma que não há suporte para o visual.
* Há suporte para **visuais personalizados** que foram **certificados**. Para obter mais informações sobre visuais personalizados certificados, incluindo como obter um visual personalizado certificado, consulte [Certificando um visual personalizado](../power-bi-custom-visuals-certified.md). Não há suporte para visuais personalizados que não foram certificados e eles são exportados como uma imagem em branco para o PowerPoint com uma mensagem de erro que afirma que não há suporte para o visual.
* No momento, não é possível exportar relatórios com mais de 30 páginas de relatório.
* O processo de exportar o relatório para o PowerPoint pode levar alguns minutos para ser concluído, seja paciente. Os fatores que podem afetar o tempo necessário incluem a estrutura do relatório e a carga atual no serviço do Power BI.
* Se o item de menu **Exportar para o PowerPoint** não estiver disponível no serviço do Power BI, provavelmente será porque seu administrador de locatários desabilitou o recurso. Entre em contato com seu administrador de locatários para obter detalhes.
* As imagens da tela de fundo serão cortadas com a área delimitadora do gráfico. É altamente recomendável que você remova as imagens de tela de fundo antes de exportar para o PowerPoint.
* As páginas no PowerPoint sempre são criadas com o tamanho padrão 9:16, independentemente do tamanho ou das dimensões da página original no relatório do Power BI.
* Os relatórios que são propriedade de um usuário fora de seu domínio de locatário do Power BI (como um relatório de alguém fora de sua organização e compartilhado com você) não podem ser publicados no PowerPoint.
* Se você compartilhar um dashboard com alguém fora de sua organização (e, portanto, um usuário que não está em seu locatário do Power BI), esse usuário não poderá exportar os relatórios associados ao dashboard compartilhado para o PowerPoint. Por exemplo, se você for aaron@contoso.com, poderá compartilhar com david@cohowinery.com. No entanto, david@cohowinery.com não poderá exportar os relatórios associados para o PowerPoint.
* Conforme mencionado anteriormente, cada página do relatório é exportada como uma única imagem no arquivo do PowerPoint.
* O serviço Power BI usa a configuração de idioma do Power BI como o idioma para a exportação do PowerPoint. Para ver ou definir sua preferência de idioma, selecione o ![ícone de engrenagem](media/end-user-powerpoint/power-bi-settings-icon.png) **> Configurações > Geral > Idioma**.
* A informação de **Baixado em** (horário) no slide capa para o arquivo exportado do PowerPoint é definido de acordo com o fuso horário do computador no momento da exportação.

## <a name="next-steps"></a>Próximas etapas
[Imprimir um relatório](end-user-print.md)
