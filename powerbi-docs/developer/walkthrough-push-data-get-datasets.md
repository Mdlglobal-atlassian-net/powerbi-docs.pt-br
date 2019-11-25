---
title: Obter um conjunto de dados para adicionar linhas
description: Passo a passo para enviar dados por push - Obter um conjunto de dados para adicionar linhas em uma tabela do Power BI
author: KesemSharabi
ms.author: kesharab
ms.reviewer: madia
ms.service: powerbi
ms.subservice: powerbi-developer
ms.topic: conceptual
ms.date: 02/05/2019
ms.openlocfilehash: a53bca63c1b0c193295a8b5c877b60ad33f5790f
ms.sourcegitcommit: c395fe83d63641e0fbd7c98e51bbab224805bbcc
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2019
ms.locfileid: "74265527"
---
# <a name="step-4-get-a-dataset-to-add-rows-into-a-power-bi-table"></a>Etapa 4: Obter um conjunto de dados para adicionar linhas em uma tabela do Power BI

Este artigo faz parte do passo a passo para [enviar dados por push a um conjunto de dados](walkthrough-push-data.md).

Na **etapa 3**, [Criar um conjunto de dados no Power BI](walkthrough-push-data-create-dataset.md), de Enviar dados por push a um conjunto de dados, você chamou a operação [Criar Conjunto de Dados](https://docs.microsoft.com/rest/api/power-bi/datasets) para criar um conjunto de dados no Power BI. Nesta etapa, você usa a operação [Obter Conjuntos de Dados](https://docs.microsoft.com/rest/api/power-bi/datasets/getdatasets) e o Newtonsoft.Json para obter uma ID de conjunto de dados. Você pode usar a ID do conjunto de dados na etapa 4 para adicionar linhas a um conjunto de dados. 

Para enviar dados por push para um conjunto de dados do Power BI, você precisa fazer referência à tabela no conjunto de dados. Para fazer referência a uma tabela em um conjunto de dados, é necessário primeiro obter uma **ID do Conjunto de Dados**. Você obtém uma **ID de Conjunto de Dados** usando a operação [Obter Conjuntos de Dados](/rest/api/power-bi/datasets/getdatasets). A operação **Obter Conjunto de Dados** retorna uma cadeia de caracteres JSON que contém uma lista de todos os conjuntos de dados no Power BI. A maneira recomendada para desserializar uma cadeia de caracteres JSON é com o [Newtonsoft.Json](https://www.newtonsoft.com/json).

Veja como obter um conjunto de dados.

## <a name="get-a-power-bi-dataset"></a>Obter um conjunto de dados do Power BI

> **OBSERVAÇÃO**: Antes de começar, lembre-se de seguir as etapas anteriores no passo a passo [enviar dados por push a um conjunto de dados](walkthrough-push-data.md).

1. No projeto de Aplicativo de Console que você criou na Etapa 2: passo a passo para enviar dados por push, [Obter um token de acesso de autenticação](walkthrough-push-data-get-token.md), instale o pacote NuGet Newtonsoft.Json. Veja como instalar o pacote:

     a. No Visual Studio 2015, escolha **Ferramentas** > **Gerenciador de Pacotes NuGet** > **Console do Gerenciador de Pacotes**.

     b. No **Console do Gerenciador de Pacotes**, digite Install-Package Newtonsoft.Json.
2. Depois de instalar o pacote, adicione **using Newtonsoft.Json;** a Program.cs.
3. Em Program.cs, adicione o código a seguir para obter uma **ID do Conjunto de Dados**.
4. Execute o Aplicativo de Console e faça logon na sua conta do Power BI. Você deve ver **ID do Conjunto de Dados:** seguido por uma ID na janela do Console.

**Exemplo de obtenção de um conjunto de dados**

Adicione este código a Program.cs.

* Em static void Main(string[] args):
  
  ```csharp
  static void Main(string[] args)
  {
  
    //Get an authentication access token
    token = GetToken();
  
    //Create a dataset in Power BI
    CreateDataset();
  
    //Get a dataset to add rows into a Power BI table
    string datasetId = GetDataset();
  }
  ```
* Adicione um método GetDatset():
  
  ```csharp
    #region Get a dataset to add rows into a Power BI table
    private static string GetDataset()
    {
        string powerBIDatasetsApiUrl = "https://api.powerbi.com/v1.0/myorg/datasets";
        //POST web request to create a dataset.
        //To create a Dataset in a group, use the Groups uri: https://api.PowerBI.com/v1.0/myorg/groups/{group_id}/datasets
        HttpWebRequest request = System.Net.WebRequest.Create(powerBIDatasetsApiUrl) as System.Net.HttpWebRequest;
        request.KeepAlive = true;
        request.Method = "GET";
        request.ContentLength = 0;
        request.ContentType = "application/json";
  
        //Add token to the request header
        request.Headers.Add("Authorization", String.Format("Bearer {0}", token));
  
        string datasetId = string.Empty;
        //Get HttpWebResponse from GET request
        using (HttpWebResponse httpResponse = request.GetResponse() as System.Net.HttpWebResponse)
        {
            //Get StreamReader that holds the response stream
            using (StreamReader reader = new System.IO.StreamReader(httpResponse.GetResponseStream()))
            {
                string responseContent = reader.ReadToEnd();
  
                //TODO: Install NuGet Newtonsoft.Json package: Install-Package Newtonsoft.Json
                //and add using Newtonsoft.Json
                var results = JsonConvert.DeserializeObject<dynamic>(responseContent);
  
                //Get the first id
                datasetId = results["value"][0]["id"];
  
                Console.WriteLine(String.Format("Dataset ID: {0}", datasetId));
                Console.ReadLine();
  
                return datasetId;
            }
        }
    }
    #endregion
  ```

A próxima etapa mostra como [adicionar linhas a uma tabela do Power BI](walkthrough-push-data-add-rows.md).

Apresentamos abaixo a [listagem de código completa](#code).

<a name="code"/>

## <a name="complete-code-listing"></a>Listagem de código completo

```csharp
using System;
using Microsoft.IdentityModel.Clients.ActiveDirectory;
using System.Net;
using System.IO;
using Newtonsoft.Json;

namespace walkthrough_push_data
{
    class Program
    {
        private static string token = string.Empty;

        static void Main(string[] args)
        {

            //Get an authentication access token
            token = GetToken();

            //Create a dataset in Power BI
            CreateDataset();

            //Get a dataset to add rows into a Power BI table
            string datasetId = GetDataset();

        }

        #region Get an authentication access token
        private static string GetToken()
        {
            // TODO: Install-Package Microsoft.IdentityModel.Clients.ActiveDirectory -Version 2.21.301221612
            // and add using Microsoft.IdentityModel.Clients.ActiveDirectory

            //The client id that Azure AD created when you registered your client app.
            string clientID = "{Client_ID}";

            //RedirectUri you used when you register your app.
            //For a client app, a redirect uri gives Azure AD more details on the application that it will authenticate.
            // You can use this redirect uri for your client app
            string redirectUri = "https://login.live.com/oauth20_desktop.srf";

            //Resource Uri for Power BI API
            string resourceUri = "https://analysis.windows.net/powerbi/api";

            //OAuth2 authority Uri
            string authorityUri = "https://login.microsoftonline.com/common/";

            //Get access token:
            // To call a Power BI REST operation, create an instance of AuthenticationContext and call AcquireToken
            // AuthenticationContext is part of the Active Directory Authentication Library NuGet package
            // To install the Active Directory Authentication Library NuGet package in Visual Studio,
            //  run "Install-Package Microsoft.IdentityModel.Clients.ActiveDirectory" from the nuget Package Manager Console.

            // AcquireToken will acquire an Azure access token
            // Call AcquireToken to get an Azure token from Azure Active Directory token issuance endpoint
            AuthenticationContext authContext = new AuthenticationContext(authorityUri);
            string token = authContext.AcquireToken(resourceUri, clientID, new Uri(redirectUri)).AccessToken;

            Console.WriteLine(token);
            Console.ReadLine();

            return token;
        }

        #endregion

        #region Create a dataset in Power BI
        private static void CreateDataset()
        {
            //TODO: Add using System.Net and using System.IO

            string powerBIDatasetsApiUrl = "https://api.powerbi.com/v1.0/myorg/datasets";
            //POST web request to create a dataset.
            //To create a Dataset in a group, use the Groups uri: https://api.PowerBI.com/v1.0/myorg/groups/{group_id}/datasets
            HttpWebRequest request = System.Net.WebRequest.Create(powerBIDatasetsApiUrl) as System.Net.HttpWebRequest;
            request.KeepAlive = true;
            request.Method = "POST";
            request.ContentLength = 0;
            request.ContentType = "application/json";

            //Add token to the request header
            request.Headers.Add("Authorization", String.Format("Bearer {0}", token));

            //Create dataset JSON for POST request
            string datasetJson = "{\"name\": \"SalesMarketing\", \"tables\": " +
                "[{\"name\": \"Product\", \"columns\": " +
                "[{ \"name\": \"ProductID\", \"dataType\": \"Int64\"}, " +
                "{ \"name\": \"Name\", \"dataType\": \"string\"}, " +
                "{ \"name\": \"Category\", \"dataType\": \"string\"}," +
                "{ \"name\": \"IsCompete\", \"dataType\": \"bool\"}," +
                "{ \"name\": \"ManufacturedOn\", \"dataType\": \"DateTime\"}" +
                "]}]}";

            //POST web request
            byte[] byteArray = System.Text.Encoding.UTF8.GetBytes(datasetJson);
            request.ContentLength = byteArray.Length;

            //Write JSON byte[] into a Stream
            using (Stream writer = request.GetRequestStream())
            {
                writer.Write(byteArray, 0, byteArray.Length);

                var response = (HttpWebResponse)request.GetResponse();

                Console.WriteLine(string.Format("Dataset {0}", response.StatusCode.ToString()));

                Console.ReadLine();
            }
        }
        #endregion

        #region Get a dataset to add rows into a Power BI table
        private static string GetDataset()
        {
            string powerBIDatasetsApiUrl = "https://api.powerbi.com/v1.0/myorg/datasets";
            //POST web request to create a dataset.
            //To create a Dataset in a group, use the Groups uri: https://api.PowerBI.com/v1.0/myorg/groups/{group_id}/datasets
            HttpWebRequest request = System.Net.WebRequest.Create(powerBIDatasetsApiUrl) as System.Net.HttpWebRequest;
            request.KeepAlive = true;
            request.Method = "GET";
            request.ContentLength = 0;
            request.ContentType = "application/json";

            //Add token to the request header
            request.Headers.Add("Authorization", String.Format("Bearer {0}", token));

            string datasetId = string.Empty;
            //Get HttpWebResponse from GET request
            using (HttpWebResponse httpResponse = request.GetResponse() as System.Net.HttpWebResponse)
            {
                //Get StreamReader that holds the response stream
                using (StreamReader reader = new System.IO.StreamReader(httpResponse.GetResponseStream()))
                {
                    string responseContent = reader.ReadToEnd();

                    //TODO: Install NuGet Newtonsoft.Json package: Install-Package Newtonsoft.Json
                    //and add using Newtonsoft.Json
                    var results = JsonConvert.DeserializeObject<dynamic>(responseContent);

                    //Get the first id
                    datasetId = results["value"][0]["id"];

                    Console.WriteLine(String.Format("Dataset ID: {0}", datasetId));
                    Console.ReadLine();

                    return datasetId;
                }
            }
        }
        #endregion
    }
}
```

[Próxima etapa >](walkthrough-push-data-add-rows.md)

## <a name="next-steps"></a>Próximas etapas

[Adicionar linhas a uma tabela do Power BI](walkthrough-push-data-add-rows.md)  
[Newtonsoft.Json](https://www.newtonsoft.com/json)  
[Obter conjuntos de dados](https://docs.microsoft.com/rest/api/power-bi/datasets/getdatasets)  
[Enviar dados por push ao Power BI](walkthrough-push-data.md)  
[Visão geral da API REST do Power BI](overview-of-power-bi-rest-api.md)  
[Referência da API REST do Power BI](https://docs.microsoft.com/rest/api/power-bi/)  

Mais perguntas? [Experimente a Comunidade do Power BI](https://community.powerbi.com/)