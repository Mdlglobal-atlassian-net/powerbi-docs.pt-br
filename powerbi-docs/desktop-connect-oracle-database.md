---
title: Conectar-se a um banco de dados Oracle
description: Etapas e downloads necessários para conectar o Oracle ao Power BI Desktop
author: davidiseminger
manager: kfile
ms.reviewer: ''
ms.service: powerbi
ms.component: powerbi-desktop
ms.topic: conceptual
ms.date: 11/28/2018
ms.author: davidi
LocalizationGroup: Connect to data
ms.openlocfilehash: 5b5dc41ee3f4d41f2e38053470054a8f453e4fb3
ms.sourcegitcommit: 2ae660a7b70fce23eb58b159d049eca44a664f2c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2018
ms.locfileid: "52670272"
---
# <a name="connect-to-an-oracle-database"></a>Conectar-se a um banco de dados Oracle
Para se conectar a um banco de dados Oracle com o **Power BI Desktop**, o software cliente Oracle correto deve estar instalado no computador que executa o Power BI Desktop. O software cliente Oracle que você usa depende de qual versão do Power BI Desktop está instalada – a versão de **32 bits** ou a de **64 bits**.

**Versões com suporte**: Oracle 9 e versões posteriores, software cliente Oracle 8.1.7 e versões posteriores.

## <a name="determining-which-version-of-power-bi-desktop-is-installed"></a>Determinando qual versão do Power BI Desktop está instalada
Para determinar qual versão do Power BI Desktop está instalada, selecione **Arquivo > Ajuda > Sobre** e, em seguida, verifique a linha **Versão:**. Na imagem a seguir, uma versão de 64 bits do Power BI Desktop está é instalada:

![](media/desktop-connect-oracle-database/connect-oracle-database_1.png)

## <a name="installing-the-oracle-client"></a>Instalando o cliente Oracle
Para versões de **32 bits** do Power BI Desktop, use o seguinte link para baixar e instalar o cliente Oracle de **32 bits**:

* [ODAC (Oracle Data Access Components) de 32 bits com Ferramentas de desenvolvimento da Oracle para Visual Studio (12.1.0.2.4)](http://www.oracle.com/technetwork/topics/dotnet/utilsoft-086879.html)

Para versões de **64 bits** do Power BI Desktop, use o seguinte link para baixar e instalar o cliente Oracle de **64 bits**:

* [ODAC de 64 bits 12c, versão 4 (12.1.0.2.4) para Windows x64](http://www.oracle.com/technetwork/database/windows/downloads/index-090165.html)

## <a name="connect-to-an-oracle-database"></a>Conectar-se a um banco de dados Oracle
Depois de instalar o driver de cliente Oracle correspondente, você pode se conectar a um banco de dados Oracle. Para fazer a conexão, execute as seguintes etapas:

1. Na janela Obter Dados, selecione **Banco de Dados > Banco de Dados Oracle**
   
   ![](media/desktop-connect-oracle-database/connect-oracle-database_2.png)
2. Na caixa de diálogo **Banco de Dados Oracle** que aparece, forneça o nome do servidor e selecione **Conectar**. Se um SID for necessário, você poderá especificá-lo usando o formato: *ServerName/SID*, em que SID é o nome exclusivo do banco de dados. Se o formato *ServerName/SID* não funcionar, tente usar *ServerName/ServiceName*, em que ServiceName é o alias usado na conexão.
   
   ![](media/desktop-connect-oracle-database/connect-oracle-database_3.png)
3. Se desejar importar dados usando uma consulta de banco de dados nativo, você pode colocar sua consulta na caixa **Instrução SQL**, disponível ao expandir a seção **Opções avançadas** da caixa de diálogo **Banco de Dados Oracle**.
   
   ![](media/desktop-connect-oracle-database/connect-oracle-database_4.png)
4. Após as informações do seu banco de dados Oracle serem inseridas na caixa de diálogo Banco de Dados Oracle (incluindo informações opcionais, como um SID ou uma consulta de banco de dados nativo), selecione **OK** para se conectar.
5. Se o banco de dados Oracle exigir credenciais de usuário do banco de dados, insira as credenciais na caixa de diálogo quando solicitado.

