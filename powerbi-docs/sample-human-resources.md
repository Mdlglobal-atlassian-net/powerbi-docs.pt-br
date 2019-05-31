---
title: 'Exemplo de recursos humanos: Faça um tour'
description: 'Exemplo de Recursos Humanos do Power BI: Faça um tour'
author: maggiesMSFT
manager: kfile
ms.reviewer: amac
ms.service: powerbi
ms.subservice: powerbi-desktop
ms.topic: conceptual
ms.date: 06/26/2018
ms.author: maggies
LocalizationGroup: Samples
ms.openlocfilehash: 4b36c02abe0ca0bbd2d117559855a69edff370db
ms.sourcegitcommit: 60dad5aa0d85db790553e537bf8ac34ee3289ba3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/29/2019
ms.locfileid: "61233638"
---
# <a name="human-resources-sample-for-power-bi-take-a-tour"></a>Exemplo de Recursos Humanos do Power BI: Faça um tour

## <a name="overview-of-the-human-resources-sample"></a>Visão geral do exemplo de Recursos Humanos
O departamento de RH tem o mesmo modelo de relatório em diferentes empresas, mesmo quando eles diferem em setor ou tamanho. Este exemplo examina novas contratações, funcionários ativos e funcionários que saíram e tenta descobrir tendências na estratégia de contratação. Nossos principais objetivos devem entender:

* Quem contratamos
* Desvios em nossa estratégia de contratação
* Tendências nas separações voluntárias

![](media/sample-human-resources/hr1.png)

Este exemplo faz parte de uma série de exemplos que ilustra como o Power BI pode ser usado com dados, relatórios e painéis orientados aos negócios. Os exemplos são dados reais de obviEnce ([www.obvience.com)](http://www.obvience.com/) que foram mantidos anônimos. Os dados estão disponíveis em vários formatos: aplicativo/pacote de conteúdo, a pasta de trabalho do Excel ou arquivo do Power BI Desktop .pbix. Para obter mais informações, confira [Conjuntos de dados de exemplo](sample-datasets.md).

## <a name="prerequisites"></a>Pré-requisitos

 Antes de usar o exemplo, primeiro você deve baixá-lo como um [pacote de conteúdo](https://docs.microsoft.com/power-bi/sample-human-resources#get-the-content-pack-for-this-sample), [arquivo pbix](http://download.microsoft.com/download/6/9/5/69503155-05A5-483E-829A-F7B5F3DD5D27/Human%20Resources%20Sample%20PBIX.pbix) ou [pasta de trabalho do Excel](http://go.microsoft.com/fwlink/?LinkId=529780).

### <a name="get-the-content-pack-for-this-sample"></a>Obter o pacote de conteúdo para este exemplo

1. Abra o serviço do Power BI (app.powerbi.com) e faça logon.
2. No canto inferior esquerdo, selecione **Obter dados**.
   
    ![](media/sample-datasets/power-bi-get-data.png)
3. Na página Obter Dados que aparece, selecione o ícone **Exemplos**.
   
   ![](media/sample-datasets/power-bi-samples-icon.png)
4. Selecione o **Exemplo de Recursos Humanos** e, em seguida, escolha **Conectar**.  
   
   ![Obter Dados](media/sample-human-resources/pbi_hr_sample_connect.png)
5. O Power BI importa o pacote de conteúdo e adiciona um novo dashboard, um relatório e um conjunto de dados ao seu workspace atual. O novo conteúdo é marcado com um asterisco amarelo. 
   
   ![Asterisco](media/sample-human-resources/human-resources-sample-asterisk.png)
  
### <a name="get-the-pbix-file-for-this-sample"></a>Obter o arquivo. pbix para este exemplo

Como alternativa, você pode baixar o exemplo como um arquivo .pbix, que é projetado para uso com o Power BI Desktop. 

 * [PBIX de exemplo de Recursos Humanos](http://download.microsoft.com/download/6/9/5/69503155-05A5-483E-829A-F7B5F3DD5D27/Human%20Resources%20Sample%20PBIX.pbix)

### <a name="get-the-excel-workbook-for-this-sample"></a>Obter a pasta de trabalho do Excel para este exemplo
Também é possível [baixar apenas o conjunto de dados (pasta de trabalho do Excel)](http://go.microsoft.com/fwlink/?LinkId=529780) para este exemplo A pasta de trabalho contém planilhas do Power View que você pode exibir e modificar. Para ver os dados brutos, selecione **Power Pivot > Gerenciar**.

## <a name="new-hires"></a>Novas contratações
Primeiro, vamos explorar as novas contratações.

1. No seu workspace, selecione a guia **Dashboards** e abra o dashboard Recursos Humanos.
2. No dashboard, selecione o bloco **Contagem de novas contratações, Novas contratações no mesmo período do ano passado, Alteração de % de YoY de funcionários ativos** **Por mês**.  
   ![](media/sample-human-resources/hr2.png)  

   O relatório de Exemplo de Recursos Humanos é aberto na página **Novas contratações** .  

   ![](media/sample-human-resources/hr3.png)

Observe o seguinte:

* O gráfico de combinação **Contagem de novas contratações, Novas contratações no mesmo período do ano passado, Alteração de % de YoY de funcionários ativos por mês** mostra que contratamos mais pessoas a cada mês neste ano, comparado ao ano passado &#151; um número significativamente maior de pessoas em alguns meses.
* No gráfico de combinação **Contagem de novas contratações e Contagem de funcionários ativos por região e etnia**, observe que estamos contratando menos pessoas na região **Leste** .
* O gráfico de cascata **Var. de YoY de novas contratações por faixa etária** mostra que estamos contratando principalmente pessoas mais jovens. Isso pode ser devido à natureza principalmente de meio período dos trabalhos.
* O gráfico de pizza **Contagem de novas contratações por gênero** mostra uma divisão bem uniforme.

Você pode encontrar mais informações, por exemplo, uma região em que a divisão de gênero não é uniforme? Selecione diferentes faixas etárias e gêneros nos gráficos para explorar as relações entre idade, gênero, região e grupo étnico.

Selecione o nome do dashboard na barra de navegação superior para retornar ao dashboard.

![](media/sample-human-resources/power-bi-breadcrumbs.png)

## <a name="compare-current-active-and-former-employees"></a>Comparar os funcionários atuais e antigos
Vamos explorar os dados de funcionários ativos atuais e funcionários que não trabalham mais na empresa.

No painel, selecione o bloco **Contagem de funcionários ativos por faixa etária** .  
![](media/sample-human-resources/pbi_hr_sample_activepie.png)

O relatório de Exemplo de Recursos Humanos é aberto na página **Funcionários ativos vs. Separações**.  
![](media/sample-human-resources/hr5.png)

**Itens de interesse**:

* Os gráficos de combinação no lado esquerdo mostraram alteração de ano a ano para funcionários ativos e separações. Temos mais ativos deste ano devido a contratação rápida, mas também mais separações do que o último ano.
* Em agosto tivemos que separar mais em comparação com outros meses. Selecione as diferentes faixas etárias, gêneros ou regiões para ver se você consegue encontrar quaisquer exceções.
* Examinando os gráficos de pizza, observamos que temos uma divisão boa, até mesmo em nossos funcionários ativos por grupos de idade e gênero. Selecione diferentes faixas etárias para ver que a divisão de gênero é distinta por idade. Temos uma divisão até mesmo por gênero em cada faixa etária?

## <a name="reasons-for-separation"></a>Motivos para separação
Abra novamente no relatório no modo de Exibição de Edição. Selecione **Editar relatório** no canto superior esquerdo.

Altere os gráficos de pizza para mostrar os dados Separados em vez de ativos.

1. Selecione o gráfico de pizza **Contagem de funcionários ativos por faixa etária** .
2. Em **Campos**, selecione a seta ao lado de **Funcionários** para expandir a tabela Funcionários. Desmarque a caixa de seleção ao lado de **Contagem de Funcionários Ativos** para remover esse campo.
3. Marque a caixa de seleção ao lado de **Contagem de separação** na tabela Funcionários para adicioná-la à caixa **Valores** bem no contêiner do campo.
4. De volta à tela do relatório, selecione a barra **Voluntário** no gráfico de barras **Contagem de separações por motivo de separação**. Isso realça os funcionários que deixaram a empresa voluntariamente nos outros visuais do relatório.
5. Clique na fatia +50 do gráfico de pizza Contagem de separações por faixa etária.

   Examine as separações pelo gráfico de linhas do Motivo no canto inferior direito. Este gráfico é filtrado para mostrar separações voluntárias.  
   ![](media/sample-human-resources/pbi_hr_sample_sepsover50.png)

   Observa a tendência no grupo etário 50+? Durante a última parte do ano, mais funcionários acima de 50 anos estão deixando a empresa voluntariamente. É uma área para investigar melhor com mais dados.
6. Você também pode seguir as mesmas etapas para o gráfico de pizza **Contagem de funcionários ativos por gênero** , alterando-o para “separações” em vez de “funcionários ativos”. Examine os dados de separação voluntário por gênero para ver se você encontrar quaisquer outras informações.
7. Clique no **Power BI** na barra de navegação superior para retornar ao painel. Você pode salvar as alterações feitas no relatório ou não.

## <a name="bad-hires"></a>Contratações incorretas
A última área para explorar são as contratações incorretas. Contratações incorretas são definidas como funcionários que não duraram mais de 60 dias. Estamos contratando rapidamente. Estamos contratando bons candidatos?

1. Selecione o bloco do painel **Contratações incorretas como % de funcionários ativos por faixa etária** . Isso abre o relatório na página 3, “Contratações Incorretas”.

   ![](media/sample-human-resources/hr7.png)  
2. Selecione a caixa de seleção **Noroeste** na segmentação Região à esquerda e a fatia **Masculino** no gráfico de rosca Contagem de Contratações Incorretas por Sexo.  Examine outros gráficos na página “Contratações Incorretas”. Mais contratações incorretas de homens do que mulheres, em muitas contratações incorretas do Grupo A.
   ![](media/sample-human-resources/pbi_hr_sample_badhirespage.png)  
3. Observando o gráfico de rosca **Contratações incorretas por gênero** e clicando na segmentação **Região** , percebemos que Leste é a Região com mais contratações incorretas de mulheres do que de homens.  
4. Selecione o nome do dashboard na barra de navegação superior para retornar ao dashboard.

## <a name="asking-a-question-in-the-qa-box"></a>Faça uma pergunta na caixa de perguntas e respostas
A [caixa de P e R](power-bi-tutorial-q-and-a.md) é onde você digita uma pergunta usando a linguagem natural. A P e R reconhece as palavras que você digita e descobre onde, em seu conjunto de dados, a resposta será encontrada.

1. Clique na caixa de P e R. Observe que, antes mesmo de começar a digitar, a caixa de P e R contém sugestões:

   ![](media/sample-human-resources/pbi_hr_sample_qabox.png)
2. Você pode escolher uma dessas sugestões ou digitar: **mostrar faixa etária, gênero e contratações incorretas no mesmo período do ano passado na região é leste**.  

   ![](media/sample-human-resources/pbi_hr_sample_qa_answer.png)

   Observe que a maioria das contratações incorretas de mulheres estão abaixo de 30 anos.

Este é um ambiente seguro para experimentar. Você pode optar por não salvar as alterações. Se você salvá-las, sempre é possível acessar **Obter Dados** para obter uma nova cópia desse exemplo.

## <a name="next-steps-connect-to-your-data"></a>Próximas etapas: Conecte-se aos seus dados
Esperamos que este tour tenha mostrado como os painéis, P e R e relatórios do Power BI podem fornecer informações sobre os dados de recursos humanos. Agora é sua vez, conecte-se aos seus próprios dados. Com o Power BI, é possível se conectar a uma grande variedade de fontes de dados. Saiba mais sobre como [começar a usar o Power BI](service-get-started.md)  
