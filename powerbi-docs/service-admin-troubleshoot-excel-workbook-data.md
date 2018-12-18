---
title: 'Erro: Não foi possível localizar nenhum dado na sua pasta de trabalho do Excel'
description: 'Erro: Não foi possível localizar nenhum dado na sua pasta de trabalho do Excel'
author: mgblythe
manager: kfile
ms.reviewer: ''
ms.service: powerbi
ms.component: powerbi-service
ms.topic: conceptual
ms.date: 12/06/2017
ms.author: mblythe
ms.custom: seodec18
LocalizationGroup: Troubleshooting
ms.openlocfilehash: ea5312178d33986ebc3f4b9e8610012c87d54216
ms.sourcegitcommit: 72c9d9ec26e17e94fccb9c5a24301028cebcdeb5
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2018
ms.locfileid: "53026021"
---
# <a name="error-we-couldnt-find-any-data-in-your-excel-workbook"></a>Erro: Não foi possível localizar nenhum dado na sua pasta de trabalho do Excel

>[!NOTE]
>Este artigo se aplica ao Excel 2007 e posterior.

Quando você importa uma pasta de trabalho do Excel para o Power BI, poderá ver o seguinte erro:

*Erro: Não foi possível encontrar nenhum dado em sua pasta de trabalho do Excel. Seus dados podem não estar formatados corretamente. Você precisará editar a pasta de trabalho no Excel e importá-la novamente.*

![Não foi possível encontrar dados na pasta de trabalho](media/service-admin-troubleshoot-excel-workbook-data/pbi_wecouldntfindanydata.png)

## <a name="quick-solution"></a>Solução rápida
1. Edite sua pasta de trabalho no Excel.
2. Selecione o intervalo de células que contém seus dados. A primeira linha deve conter seus cabeçalhos de coluna (os nomes de coluna).
3. Pressione **Ctrl + T** para criar uma tabela.
4. Salve sua pasta de trabalho.
5. Retorne ao Power BI e importe sua pasta de trabalho novamente, ou se estiver trabalhando no Excel 2016 e salvou a pasta de trabalho no OneDrive para Empresas, no Excel, clique em Arquivo > Publicar.

## <a name="details"></a>Detalhes
### <a name="cause"></a>Causa
No Excel, você pode criar uma **tabela** fora de um intervalo de células, o que torna mais fácil classificar, filtrar e formatar dados.

Quando você importa uma pasta de trabalho do Excel, o Power BI procura essas tabelas e as importa para um conjunto de dados; se ele não encontrar todas as tabelas, você verá essa mensagem de erro.

### <a name="solution"></a>Solução
1. Abra sua pasta de trabalho no Excel. 
    >[!NOTE]
    >As imagens aqui exibidas são do Excel 2013. Se você estiver usando outra versão, a aparência poderá ser um pouco diferente, mas as etapas são as mesmas.
    
    ![Abrir pasta de trabalho](media/service-admin-troubleshoot-excel-workbook-data/pbi_trb_xlwksht1.png)
2. Selecione o intervalo de células que contém seus dados. A primeira linha deve conter seus cabeçalhos de coluna (os nomes de coluna):
   
    ![Selecionar intervalo de células](media/service-admin-troubleshoot-excel-workbook-data/pbi_trb_xlwksht2.png)
3. Na faixa de opções da guia **INSERIR** , clique em **Tabela**. (Ou, como um atalho, pressione **Ctrl + T**.)
   
    ![Inserir tabela](media/service-admin-troubleshoot-excel-workbook-data/pbi_trb_xlwksht3.png)
4. Você verá a caixa de diálogo a seguir. Certifique-se de que a opção **Minha tabela tem títulos** está marcada e selecione **OK**:
   
    ![Criar tabela](media/service-admin-troubleshoot-excel-workbook-data/pbi_trb_xlcreatetbl.png)
5. Agora que seus dados estão formatados como uma tabela:
   
    ![Dados formatados como uma tabela](media/service-admin-troubleshoot-excel-workbook-data/pbi_trb_xltbl.png)
6. Salve sua pasta de trabalho.
7. Volte para o Power BI. Selecione Obter Dados na parte inferior do painel de navegação esquerdo.
   
    ![Obter dados](media/service-admin-troubleshoot-excel-workbook-data/pbi_getdata.png)
8. Na caixa **Arquivos** , selecione **Obter**.
   
    ![Obter arquivos](media/service-admin-troubleshoot-excel-workbook-data/pbi_getfiles.png)
9. Importe novamente sua pasta de trabalho do Excel. Desta vez, a importação deve localizar a tabela e ser realizada com êxito.
   
    Se a importação ainda falhar, fale conosco clicando em **Comunidade** no menu Ajuda:
   
    ![Link da comunidade](media/service-admin-troubleshoot-excel-workbook-data/pbi_questionmenucommunity.png)
