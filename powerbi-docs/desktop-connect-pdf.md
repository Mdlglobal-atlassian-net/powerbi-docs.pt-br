---
title: Conectar a um arquivo PDF no Power BI Desktop
description: Conecte-se facilmente e use dados de arquivos PDF no Power BI Desktop
author: davidiseminger
manager: kfile
ms.reviewer: ''
ms.service: powerbi
ms.subservice: powerbi-desktop
ms.topic: conceptual
ms.date: 05/08/2019
ms.author: davidi
LocalizationGroup: Connect to data
ms.openlocfilehash: 0c63a62edfce62a5cee13bef3c68014027313e8b
ms.sourcegitcommit: 60dad5aa0d85db790553e537bf8ac34ee3289ba3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/29/2019
ms.locfileid: "65514038"
---
# <a name="connect-to-a-pdf-file-in-power-bi-desktop"></a>Conectar a um arquivo PDF no Power BI Desktop
No Power BI Desktop, é possível se conectar a um **arquivo PDF** e usar os dados incluídos do arquivo, como qualquer outra fonte de dados no Power BI Desktop.

![Conectar-se aos dados em arquivos PDF](media/desktop-connect-pdf/connect-pdf_04.png)

As seguintes seções descrevem como conectar-se a um **arquivo PDF**, selecionar dados e trazê-los para o **Power BI Desktop**.

É recomendável sempre atualizar para a versão mais recente do **Power BI Desktop**, que pode ser obtida de um link em [obter o Power BI Desktop](desktop-get-the-desktop.md). 

## <a name="connect-to-a-pdf-file"></a>Conectar-se a um arquivo PDF
Para se conectar a um arquivo **PDF**, selecione **Obter dados** na faixa de opções **Início** no Power BI Desktop. Selecione **Arquivo** nas categorias à esquerda e você verá o **PDF (beta)** .

![Selecionar PDF em Obter dados](media/desktop-connect-pdf/connect-pdf_01.png)

Você deverá fornecer o local do arquivo PDF que deseja usar. Após fornecer o local do arquivo e o carregamento do arquivo PDF, uma janela **Navegador** aparecerá e exibirá os dados disponíveis do arquivo, na qual será possível selecionar um ou vários elementos para serem importados e usados no **Power BI Desktop**.

![Conectar-se aos dados em arquivos PDF](media/desktop-connect-pdf/connect-pdf_04.png)

Marcar uma caixa de seleção ao lado de elementos descobertos no arquivo PDF exibe-os no painel direito. Quando estiver pronto para importar, selecione o botão **Carregar** para inserir os dados no **Power BI Desktop**.

A partir da versão de novembro de 2018 do **Power BI Desktop**, você pode especificar a **Página inicial** e **Página final** como parâmetros opcionais para sua conexão de PDF. Você também pode especificar esses parâmetros na linguagem de fórmula M, usando o seguinte formato:

`Pdf.Tables(File.Contents("c:\sample.pdf"), [StartPage=10, EndPage=11])`


## <a name="next-steps"></a>Próximas etapas
Há todos os tipos de dados aos quais você pode se conectar usando o Power BI Desktop. Para obter mais informações sobre fontes de dados, confira os seguintes recursos:

* [O que é o Power BI Desktop?](desktop-what-is-desktop.md)
* [Fontes de dados no Power BI Desktop](desktop-data-sources.md)
* [Formatar e combinar dados com o Power BI Desktop](desktop-shape-and-combine-data.md)
* [Conectar-se a pastas de trabalho do Excel no Power BI Desktop](desktop-connect-excel.md)   
* [Inserir dados diretamente no Power BI Desktop](desktop-enter-data-directly-into-desktop.md)   

