---
title: Novidades no Servidor de Relatório do Power BI
description: Saiba quais são as novidades no Servidor de Relatório do Power BI. Elas abrangem as principais áreas de recurso e são atualizadas conforme novos itens são lançados.
author: maggiesMSFT
ms.author: maggies
manager: kfile
ms.reviewer: ''
ms.service: powerbi
ms.subservice: powerbi-report-server
ms.topic: conceptual
ms.date: 05/22/2019
ms.openlocfilehash: 364795a25aaffb92afc4a7148c9bf6b3f88d2ac8
ms.sourcegitcommit: 60dad5aa0d85db790553e537bf8ac34ee3289ba3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/29/2019
ms.locfileid: "66187307"
---
# <a name="whats-new-in-power-bi-report-server"></a>Novidades no Servidor de Relatório do Power BI

Saiba mais sobre o que há de novo no servidor de relatório do Power BI e Power BI Desktop otimizado para o servidor de relatório do Power BI. Este artigo aborda as principais áreas de recursos e é atualizado conforme novos itens são lançados.

Para saber mais sobre as “Novidades” do Power BI, consulte:

* [Novidades no serviço do Power BI](../service-whats-new.md)
* [Novidades no Power BI Desktop](../desktop-latest-update.md)
* [Novidades em aplicativos móveis para o Power BI](../consumer/mobile/mobile-whats-new-in-the-mobile-apps.md)

## <a name="may-2019-power-bi-desktop-for-power-bi-report-server"></a>Maio de 2019: Área de trabalho do Power BI para Power BI Report Server

Consulte a [servidor de relatório do Power BI de maio de 2019](https://powerbi.microsoft.com/blog/power-bi-report-server-update-may-2019/) postagem de blog para obter detalhes sobre os novos recursos.

Aqui estão alguns dos destaques da versão:

### <a name="performance-analyzer"></a>Analisador de desempenho 

Se o relatório é executado mais lentamente do que o esperado, tente o analisador de desempenho no Power BI Desktop. Quando você iniciá-lo, ele cria um arquivo de log com informações sobre cada ação realizada no relatório. Leia mais sobre o [Performance Analyzer](../desktop-performance-analyzer.md).

### <a name="new-modeling-view"></a>Novo modo de exibição de modelagem

Na nova exibição de modelagem no Power BI Desktop, você pode exibir e trabalhar com conjuntos de dados complexos que contêm muitas tabelas. Destaques incluem vários layouts de diagrama e em massa de edição de colunas, medidas e tabelas. Leia mais sobre [exibição da modelagem](../desktop-modeling-view.md).

### <a name="accessible-visual-interaction"></a>Interação visual acessível

Você pode agora pontos de dados de acesso em muitos dos visuais internos usando a navegação de teclado. Leia mais sobre [acessibilidade nos relatórios do Power BI](../desktop-accessibility.md).

### <a name="conditional-formatting-titles-and-web-url-actions"></a>Formatação de títulos e ações de URL da web condicional

Relatórios do Power BI são interativos. Faz sentido que os títulos em um relatório seria dinâmicos, para refletir o estado atual do relatório. Você pode usar a mesma expressão ligada à formatação para tornar as URLs de imagens, formas e botões dinâmicos. Leia mais sobre [baseadas em expressão títulos](../desktop-conditional-format-visual-titles.md).

### <a name="cross-highlight-by-axis-labels"></a>Realce cruzado por rótulos de eixo

Selecione os rótulos de eixo de categoria em um visual para os outros elementos em uma página, realce cruzado, exatamente como você selecionaria os pontos de dados em um visual. Leia mais sobre [realce cruzado](../power-bi-reports-filters-and-highlighting.md#ad-hoc-highlighting).

### <a name="all-the-new-features"></a>Todos os novos recursos

Aqui está a lista de todos os novos recursos:

### <a name="reporting"></a>Relatórios

- Realce cruzado em um único ponto em gráficos de linhas 
- Quebra automática de linha em títulos 
- Atualizar interação visual padrão para filtro cruzado ¬
- Cantos arredondados para bordas visuais 
- Selecione segmentação de dados única  
- Suporte ao mapa de calor para o Bing maps  
- Realce cruzado por rótulos de eixo  
- Dica de ferramenta padrão de formatação  
- Suporte de URL com a web estático para botões, imagens e formas  
- Opções de alinhamento de página   
- Aprimoramentos do painel de seleção  
- Interação visual acessível  
- Formatação de títulos de visuais condicional  
- Formatação para ações de URL da web para botões, imagens e formas condicional
- Painel do analisador de desempenho
- Navegação de teclado de tabela e matriz
- Controle de posição de rótulo de dados de linha
- Controle de tamanho de texto de indicador visual de KPI

### <a name="analytics"></a>Análise

- Mostrar datas como uma hierarquia geralmente disponível  

### <a name="modeling"></a>Modelagem

- Modelagem novo modo de exibição já está disponível
- Novas funções do DAX
- Atualizar para a função ALLSELECTED DAX
- Desabilitar as tabelas de data automática de novos relatórios

## <a name="may-2019-power-bi-report-server"></a>Maio de 2019: Servidor de Relatórios do Power BI

### <a name="support-for-trusted-visuals"></a>Suporte para visuais confiáveis

Adicionamos suporte para visuais confiável no servidor de relatório do Power BI. Atualmente, damos suporte a elementos visuais Mapbox e PowerOn. ESRI, Visio e o PowerApps não têm suporte para esta versão.)

### <a name="improved-security-features"></a>Recursos de segurança aprimorada

**RestrictedResourceMimeTypeForUpload**, quais os administradores podem usar para especificar uma lista separada por vírgulas de tipos de mime proibidos, por exemplo, texto/html.

## <a name="january-2019"></a>Janeiro de 2019

Suporte para esses recursos em relatórios do Power BI:

[**Segurança em nível de linha**](row-level-security-report-server.md) Configurar a RLS (Segurança em Nível de Linha) com o Servidor de Relatórios do Microsoft Power BI pode restringir acesso a dados para determinados usuários. Os filtros restringem o acesso a dados no nível da linha e você pode definir filtros nas funções.

[**Expandir e recolher os cabeçalhos de linha de matriz**](https://powerbi.microsoft.com/blog/power-bi-desktop-november-2018-feature-summary/#expandCollapse) Adicionamos a capacidade de expandir e recolher cabeçalhos de linha individuais, um dos recursos visuais mais solicitados.

[**Copiar e colar entre arquivos .pbix**](https://powerbi.microsoft.com/blog/power-bi-desktop-november-2018-feature-summary/#copyPaste) Você pode copiar os elementos visuais entre arquivos .pbix, no menu de contexto do visual ou com o atalho de teclado Ctrl + C padrão e colá-los em outro relatório com Ctrl + V.

[**Guias de alinhamento inteligentes**](https://powerbi.microsoft.com/blog/power-bi-desktop-december-2018-feature-summary/#smartGuides) Você vê guias de alinhamento inteligentes ao mover objetos na sua página de relatório, assim como você vê no PowerPoint, para ajudá-lo a alinhar tudo na sua página. Você vê as guias inteligentes sempre que você arrasta ou redimensiona algo na página. Quando você move um objeto para perto de outro, ele se ajusta em uma posição alinhada com o outro objeto.

**Recursos de acessibilidade** Há muitos recursos de acessibilidade para listar: por exemplo, [suporte de acessibilidade do painel de lista de campos](https://powerbi.microsoft.com/blog/power-bi-desktop-december-2018-feature-summary/#fieldList). O painel de lista de campos é totalmente acessível. Você pode navegar pelo painel usando apenas o teclado e um leitor de tela e usar o menu de contexto para adicionar campos à sua página de relatório.

#### <a name="custom-visuals"></a>Visuais Personalizados

- A versão da API fornecida com esta versão é a 2.3.

### <a name="administrator-settings"></a>Configurações do administrador

Os administradores podem definir as seguintes propriedades nas Propriedades Avançadas do SSMS para o farm de servidores:

**AllowedResourceExtensionsForUpload** Definir extensões de recursos que podem ser carregados para o servidor de relatório. Extensões para tipos de arquivo internos, como &ast;.rdl e &ast;.pbix não devem ser incluídos. O padrão é "&ast;, &ast;.xml, &ast;.xsd, &ast;.xsl, &ast;.png, &ast;.gif, &ast;.jpg, &ast;.tif, &ast;.jpeg, &ast;.tiff, &ast;.bmp, &ast;.pdf, &ast;.svg, &ast;.rtf, &ast;.txt, &ast;.doc, &ast;.docx, &ast;.pps, &ast;.ppt, &ast;.pptx". 

**SupportedHyperlinkSchemes** Define uma lista separada por vírgulas dos esquemas de URI que têm permissão para serem definidos em ações de hiperlink que têm permissão para serem processados ou então "&ast;" para habilitar todos os esquemas de hiperlink. Por exemplo, definir "http,https" permitiria hiperlinks para "https://www. contoso.com", mas removeria hiperlinks para "mailto:bill@contoso.com" ou "javascript:window.open(‘www.contoso.com’, ‘_blank’)". O padrão é "&ast;".

## <a name="august-2018"></a>Agosto de 2018

Em agosto de 2018, vários novos recursos foram adicionados à versão do Power BI Desktop otimizada para o Servidor de Relatórios do Power BI. Aqui estão elas, divididas por área:

- [Relatórios](#reporting)
- [Análise](#analytics)
- [Modelagem](#modeling)

### <a name="highlights-of-the-august-2018-release"></a>Destaques da versão de agosto de 2018

De toda a longa lista de novos recursos, estes se destacam por serem mais interessantes. Para obter mais informações, confira nossa [postagem no blog](https://powerbi.microsoft.com/blog/power-bi-report-server-update-august-2018/).

#### <a name="report-theming"></a>Tema do relatório

O tema do relatório foi adicionado à versão de agosto de 2018 do Servidor de Relatórios do Power BI, que permite colorir rapidamente o relatório inteiro para corresponder a um tema ou à identidade visual da empresa. Quando você importa um tema, todos os gráficos são atualizados automaticamente para usar as cores do tema e você pode ter acesso às cores do tema na paleta de cores. Você pode carregar um arquivo de tema usando a opção **Importar Tema** no botão **Mudar Tema**.

Um arquivo de tema é um arquivo JSON que inclui todas as cores que você deseja usar em seu relatório, juntamente com qualquer formatação padrão que deseja aplicar aos visuais.
Aqui está um exemplo simples de tema JSON que apenas atualiza as cores padrão do relatório:

```json
{
"name": "waveform",
"dataColors": [ "#31B6FD", "#4584D3", "#5BD078", "#A5D028", "#F5C040", "#05E0DB", "#3153FD", "#4C45D3", "#5BD0B0", "#54D028", "#D0F540", "#057BE0" ],
"background":"#FFFFFF",
"foreground": "#F2F2F2",
"tableAccent":"#5BD078"
}
```

#### <a name="conditional-formatting-by-a-different-field"></a>Formatação condicional usando um campo diferente

A capacidade de formatar uma coluna usando um campo diferente em seu modelo é uma das melhorias significativas da formatação condicional.

#### <a name="conditional-formatting-by-values"></a>Formatação condicional usando valores

Outro tipo novo de formatação condicional é o valor **Formatar por campo**. O valor Formatar por campo permite usar uma medida ou coluna que especifica uma cor, por meio de um código hexadecimal ou um nome, e aplica essa cor à cor da tela de fundo ou da fonte.

#### <a name="report-page-tooltips"></a>Dicas de ferramentas de página de relatório

O recurso de dicas de ferramenta da página de relatório foi incluído na atualização de agosto de 2018 do Servidor de Relatórios do Power BI. Esse recurso permite criar uma página de relatório a ser usada como uma dica de ferramenta personalizada para outros visuais no relatório.

#### <a name="log-axis-improvements"></a>Melhorias do eixo logarítmico

Melhoramos consideravelmente o eixo logarítmico em seus gráficos cartesianos. Agora, você pode selecionar a escala logarítmica do eixo numérico de qualquer gráfico cartesiano, incluindo o gráfico de combinação, quando houver dados completamente positivos ou completamente negativos.

#### <a name="sap-hana-sso-direct-query"></a>DirectQuery de SSO do SAP HANA

O suporte para DirectQuery de SSO do SAP HANA com o Kerberos já está disponível para relatórios do Power BI.

>[!Note]
>Há suporte para esse cenário apenas quando o SAP HANA é tratado como uma fonte de dados relacional com os relatórios que você criou no Power BI Desktop.  Para habilitar isso no Power BI Desktop, no menu do DirectQuery, em Opções, marque "Tratar SAP HANA como uma fonte relacional" e clique em OK.

#### <a name="custom-visuals"></a>Visuais Personalizados

- A versão da API fornecida com esta versão é a 1.13.0.

- Agora, os visuais personalizados podem voltar a uma versão anterior compatível com a versão atual da API do servidor (se disponível).

### <a name="reporting"></a>Relatórios 

- [Tema do relatório](https://powerbi.microsoft.com/blog/power-bi-report-server-update-august-2018/#theming)
- [Botões para disparar ações](https://powerbi.microsoft.com/blog/power-bi-report-server-update-august-2018/#buttons)
- [Estilos de linha do gráfico de combinação](https://powerbi.microsoft.com/blog/power-bi-report-server-update-august-2018/#comboLines)
- [Melhor classificação padrão para visuais](https://powerbi.microsoft.com/blog/power-bi-report-server-update-august-2018/#sort)
- [Segmentação numérica](https://powerbi.microsoft.com/blog/power-bi-report-server-update-august-2018/#numericSlicer)
- [Sincronizando de segmentação avançada](https://powerbi.microsoft.com/blog/power-bi-report-server-update-august-2018/#slicerSync)
- [Melhorias do eixo logarítmico](https://powerbi.microsoft.com/blog/power-bi-report-server-update-august-2018/#logAxis)
- [Opções de rótulo de dados para gráfico de funil](https://powerbi.microsoft.com/blog/power-bi-report-server-update-august-2018/#funnelChart)
- [Definir a largura do traço da linha para zero](https://powerbi.microsoft.com/blog/power-bi-report-server-update-august-2018/#lineStroke)
- [Suporte para alto contraste em relatórios](https://powerbi.microsoft.com/blog/power-bi-report-server-update-august-2018/#highContrast)
- [Controle de raio de rosca](https://powerbi.microsoft.com/blog/power-bi-report-server-update-august-2018/#donutRadius)
- [Controle de posição de rótulos de detalhe de pizza e rosca](https://powerbi.microsoft.com/blog/power-bi-report-server-update-august-2018/#detailLabels)
- [Formatar rótulos de dados separadamente para cada medida em um gráfico de combinação](https://powerbi.microsoft.com/blog/power-bi-report-server-update-august-2018/#comboLabels)
- [Novo cabeçalho visual com mais flexibilidade e formatação](https://powerbi.microsoft.com/blog/power-bi-report-server-update-august-2018/#visualHeader)
- [Formatação de papel de parede](https://powerbi.microsoft.com/blog/power-bi-report-server-update-august-2018/#wallpaper)
- [Dicas de ferramentas de tabela e de matriz](https://powerbi.microsoft.com/blog/power-bi-report-server-update-august-2018/#tableTooltips)
- [Desabilitar as dicas de ferramentas de visuais](https://powerbi.microsoft.com/blog/power-bi-report-server-update-august-2018/#tooltips)
- [Acessibilidade de segmentação](https://powerbi.microsoft.com/blog/power-bi-report-server-update-august-2018/#slicerAccessibility)
- [Melhorias do painel de formatação](https://powerbi.microsoft.com/blog/power-bi-report-server-update-august-2018/#formattingPane)
- [Suporte para linha de nível em gráficos de linhas e de combinação](https://powerbi.microsoft.com/blog/power-bi-report-server-update-august-2018/#steppedLine)
- [Melhoria da experiência de classificação](https://powerbi.microsoft.com/blog/power-bi-report-server-update-august-2018/#sorting)
- [Imprimir relatórios por meio da Exportação para PDF (no Power BI Desktop)](https://powerbi.microsoft.com/blog/power-bi-report-server-update-august-2018/#print)
- [Criar grupos de indicadores](https://powerbi.microsoft.com/blog/power-bi-report-server-update-august-2018/#bookmarks)
- [Redefinição de segmentação](https://powerbi.microsoft.com/blog/power-bi-report-server-update-august-2018/#slicer)
- [Dicas de ferramenta da página de relatório](https://powerbi.microsoft.com/blog/power-bi-report-server-update-august-2018/#reportPageTooltips)

### <a name="analytics"></a>Análise

- [Nova função DAX: COMBINEVALUES()](https://powerbi.microsoft.com/blog/power-bi-report-server-update-august-2018/#combineValues)
- [Detalhamento de medida](https://powerbi.microsoft.com/blog/power-bi-report-server-update-august-2018/#measureDrillthrough)
- [Formatação condicional usando um campo diferente](https://powerbi.microsoft.com/blog/power-bi-report-server-update-august-2018/#conditionalFormattingField)
- [Formatação condicional usando valores](https://powerbi.microsoft.com/blog/power-bi-report-server-update-august-2018/#conditionalFormattingValue)

### <a name="modeling"></a>Modelagem

- [Filtragem e classificação na exibição de dados](https://powerbi.microsoft.com/blog/power-bi-report-server-update-august-2018/#filterAndSort)
- [Melhoria na formatação de localidade](https://powerbi.microsoft.com/blog/power-bi-report-server-update-august-2018/#locale)
- [Categorias de dados para medidas](https://powerbi.microsoft.com/blog/power-bi-report-server-update-august-2018/#dataCategory)
- [Funções estatísticas do DAX](https://powerbi.microsoft.com/blog/power-bi-report-server-update-august-2018/#dax)

## <a name="may-2018"></a>Mai 2018

### <a name="configure-power-bi-ios-mobile-apps-for-report-servers-remotely"></a>Configurar aplicativos móveis do Power BI iOS para servidores de relatório remotamente

Como um administrador de TI, agora é possível usar ferramenta MDM da sua organização para configurar remotamente o acesso de aplicativo móvel do Power BI iOS a um servidor de relatório. Confira [Configurar o acesso do aplicativo móvel do Power BI iOS a um servidor de relatório remotamente](configure-powerbi-mobile-apps-remote.md) para obter detalhes.

## <a name="march-2018"></a>Março de 2018

Em março de 2018, houve a adição de muitos recursos novos à versão do Power BI Desktop otimizado para o Servidor de Relatórios do Power BI. Aqui estão elas, divididas por área:

- [Visuais](#visuals-updates)
- [Relatórios](#reporting)
- [Análise](#analytics)
- [Desempenho](#performance)
- [Servidor de relatórios](#report-server)
- [Outros](#other-improvements)

### <a name="highlights-of-the-march-2018-release"></a>Destaques da versão de março de 2018

De toda a longa lista de novos recursos, estes se destacam por serem mais interessantes.

#### <a name="rule-based-conditional-formatting-for-table-and-matrixhttpspowerbimicrosoftcomblogpower-bi-desktop-november-2017-feature-summaryconditionalformatting"></a>[Formatação condicional baseada em regras para visuais de tabela e de matriz](https://powerbi.microsoft.com/blog/power-bi-desktop-november-2017-feature-summary/#conditionalFormatting)

Crie regras para colorir condicionalmente a tela de fundo ou a fonte de uma coluna com base na lógica de negócios específica na tabela ou na matriz.

#### <a name="show-and-hide-pageshttpspowerbimicrosoftcomblogpower-bi-desktop-january-2018-feature-summaryhidepages"></a>[Mostrar e ocultar páginas](https://powerbi.microsoft.com/blog/power-bi-desktop-january-2018-feature-summary/#hidePages)

Você deseja que os leitores acessem seu relatório, mas algumas páginas não estão concluídas. Agora você pode ocultá-las até que elas fiquem prontas. Ou você pode ocultar páginas da navegação normal, permitindo que os leitores cheguem à página por indicadores ou por detalhamento.

#### <a name="bookmarkinghttpspowerbimicrosoftcomblogpower-bi-desktop-march-2018-feature-summarybookmarking"></a>[Uso de indicadores](https://powerbi.microsoft.com/blog/power-bi-desktop-march-2018-feature-summary/#bookmarking)

Falando de uso de indicadores, crie-os para contar uma história com os dados em seu relatório.

- [Realce cruzado para indicadores](https://powerbi.microsoft.com/blog/power-bi-desktop-december-feature-summary/#bookmarkCrossHighlighting): indicadores mantêm e exibem o estado com realce cruzado da página do relatório no momento em que são criados.
- [Mais flexibilidade para indicadores](https://powerbi.microsoft.com/blog/power-bi-desktop-december-feature-summary/#bookmarkFlexibility): indicadores refletem as propriedades que você define no relatório e afeta somente os visuais que você escolhe.

#### <a name="multi-select-data-points-across-multiple-chartshttpspowerbimicrosoftcomblogpower-bi-desktop-february-2018-feature-summarycrosshighlight"></a>[Pontos de dados de seleção múltipla em vários gráficos](https://powerbi.microsoft.com/blog/power-bi-desktop-february-2018-feature-summary/#crosshighlight)

Selecione vários pontos de dados em vários gráficos e aplique a filtragem cruzada a toda a página.

#### <a name="sync-slicers-across-multiple-pages-of-your-reporthttpspowerbimicrosoftcomblogpower-bi-desktop-february-2018-feature-summarysyncslicers"></a>[Sincronizar segmentações de dados em várias páginas do relatório](https://powerbi.microsoft.com/blog/power-bi-desktop-february-2018-feature-summary/#syncSlicers)

Uma segmentação de dados pode se aplicar a uma, duas ou mais páginas em um relatório.

#### <a name="quick-measureshttpspowerbimicrosoftcomblogpower-bi-desktop-february-2018-feature-summaryquickmeasures"></a>[Medidas rápidas](https://powerbi.microsoft.com/blog/power-bi-desktop-february-2018-feature-summary/#quickMeasures) 

Crie medidas com base em medidas existentes e nas colunas numéricas em uma tabela.

#### <a name="drilling-down-filters-other-visualshttpspowerbimicrosoftcomblogpower-bi-desktop-december-feature-summarydrillfiltersothervisuals"></a>[Filtros de detalhamento de outros elementos visuais](https://powerbi.microsoft.com/blog/power-bi-desktop-december-feature-summary/#drillFiltersOtherVisuals)

Quando você faz drill down em uma determinada categoria em um visual, você pode filtrar todos os elementos visuais na página por essa mesma categoria.

### <a name="visuals-updates"></a>Atualizações de visuais

- [Alinhamento de células para visuais de tabela e de matriz](https://powerbi.microsoft.com/blog/power-bi-desktop-november-2017-feature-summary/#alignment)
- [Ver unidades e controle de precisão para colunas de tabela e de matriz](https://powerbi.microsoft.com/blog/power-bi-desktop-march-2018-feature-summary/#displayUnits)
- [Rótulos de dados de estouro para elementos visuais de gráfico de barras e colunas](https://powerbi.microsoft.com/blog/power-bi-desktop-february-2018-feature-summary/#overflow)
- [Controlar a cor da tela de fundo do rótulo de dados para Cartesiano e visuais de mapas](https://powerbi.microsoft.com/blog/power-bi-desktop-january-2018-feature-summary/#dataLabelBackground)
- [Controle de preenchimento de barra/coluna](https://powerbi.microsoft.com/blog/power-bi-desktop-january-2018-feature-summary/#padding)
- [Aumentar a área usada para rótulos de eixo em gráficos](https://powerbi.microsoft.com/blog/power-bi-desktop-january-2018-feature-summary/#axisSize)
- [Dispersão visual de agrupamentos do eixo x e y](https://powerbi.microsoft.com/blog/power-bi-desktop-december-feature-summary/#scatterChart)
- [Amostragem de alta densidade para mapas com base em latitude e longitude](https://powerbi.microsoft.com/blog/power-bi-desktop-december-feature-summary/#highDensityMaps)
- [Segmentações responsivas](https://powerbi.microsoft.com/blog/power-bi-desktop-december-feature-summary/#responsive)
- [Adicionar uma data de âncora para segmentação de data relativa](https://powerbi.microsoft.com/blog/power-bi-desktop-january-2018-feature-summary/#anchorDate)

### <a name="reporting"></a>Relatórios

- [Desativar o cabeçalho do visual no modo de leitura em um relatório](https://powerbi.microsoft.com/blog/power-bi-desktop-march-2018-feature-summary/#visualHeader)
- [Opções de relatório para fontes de dados lentas](https://powerbi.microsoft.com/blog/power-bi-desktop-november-2017-feature-summary/#slowDataSource)
- [Posicionamento de visual padrão aprimorado](https://powerbi.microsoft.com/blog/power-bi-desktop-march-2018-feature-summary/#visualPlacement)
- [Controle a ordem visual por meio do painel de seleção](https://powerbi.microsoft.com/blog/power-bi-desktop-november-2017-feature-summary/#selectionPane)
- [Bloqueie objetos no relatório](https://powerbi.microsoft.com/blog/power-bi-desktop-november-2017-feature-summary/#lock)
- [Pesquisar o painel de formatação e análise](https://powerbi.microsoft.com/blog/power-bi-desktop-february-2018-feature-summary/#search)
- [Painel de propriedades de campo e descrições de campo](https://powerbi.microsoft.com/blog/power-bi-desktop-december-feature-summary/#fieldPropertiesPane)

### <a name="analytics"></a>Análise

- [UTCNOW() e UTCTODAY()](https://powerbi.microsoft.com/blog/power-bi-desktop-february-2018-feature-summary/#utcDAX)
- [Marcar tabela de datas personalizada](https://powerbi.microsoft.com/blog/power-bi-desktop-february-2018-feature-summary/#customDateTable)
- [Detalhar filtros de outros visuais](https://powerbi.microsoft.com/blog/power-bi-desktop-december-feature-summary/#drillFiltersOtherVisuals)
- [Formatação de nível de célula para modelos multidimensionais do AS para cartão de múltiplas linhas](https://powerbi.microsoft.com/blog/power-bi-desktop-november-2017-feature-summary/#cellLevelFormatting)

### <a name="performance"></a>Desempenho

- [Melhorias de desempenho de filtragem](https://powerbi.microsoft.com/blog/power-bi-desktop-november-2017-feature-summary/#filtering)
- [Melhorias de desempenho DirectQuery](https://powerbi.microsoft.com/blog/power-bi-desktop-february-2018-feature-summary/#dqPerf)
- [Melhorias de desempenho de abrir e salvar](https://powerbi.microsoft.com/blog/power-bi-desktop-february-2018-feature-summary/#savePerf)
- [Melhorias de “Mostrar itens sem dados”](https://powerbi.microsoft.com/blog/power-bi-desktop-february-2018-feature-summary/#showItemsWithNoData)

### <a name="report-server"></a>Servidor de relatórios

#### <a name="export-to-accessible-pdf"></a>Exportar para PDF acessível

Quando você exporta um relatório paginado (RDL) para PDF, você pode obter um arquivo PDF acessível/marcado. Ele é maior em tamanho, mas sua leitura e navegação pelos leitores de tela e outras tecnologias assistenciais é mais fácil. Você habilita o PDF acessível definindo a configuração de informações de dispositivo **AccessiblePDF** para **True**. Consulte [Configuração de Informações de Dispositivo PDF](https://docs.microsoft.com/sql/reporting-services/pdf-device-information-settings) e [Alterar as Configurações de Informações do Dispositivo](https://docs.microsoft.com/sql/reporting-services/customize-rendering-extension-parameters-in-rsreportserver-config#changing-device-information-settings).

### <a name="other-improvements"></a>Outros aprimoramentos

- [Aprimoramentos em Adicionar Coluna de Exemplos](https://powerbi.microsoft.com/blog/power-bi-desktop-november-2017-feature-summary/#addColumnFromExamples)
- [Link rápido para Serviços de Consultoria](https://powerbi.microsoft.com/blog/power-bi-desktop-february-2018-feature-summary/#consultingServices)
- [Relatório de erros aprimorado](https://powerbi.microsoft.com/blog/power-bi-desktop-march-2018-feature-summary/#errors)
- [Ver erros anteriores que você encontrou](https://powerbi.microsoft.com/blog/power-bi-desktop-march-2018-feature-summary/#viewErrors)

## <a name="october-2017"></a>Outubro de 2017

### <a name="power-bi-report-data-sources"></a>Fontes de dados de relatório do Power BI

Os relatórios do Power BI no Servidor de Relatórios do Power BI podem conectar-se a uma variedade de fontes de dados. É possível importar e agendar a atualização de dados ou consultá-los diretamente usando o DirectQuery ou uma conexão dinâmica ao SQL Server Analysis Services. Veja a lista das fontes de dados compatíveis com a atualização agendada e as compatíveis com o DirectQuery em "Fontes de dados de relatórios do Power BI no Servidor de Relatórios do Power BI".

### <a name="scheduled-data-refresh-for-imported-data"></a>Atualização agendada de dados importados

No Servidor de Relatórios do Power BI, é possível configurar a atualização de dados agendada para manter os dados atualizados nos relatórios do Power BI usando um modelo inserido, em vez de uma conexão dinâmica ou o DirectQuery. Com um modelo inserido, os dados importados estão desconectados da fonte de dados original. Eles precisam ser atualizados para permanecerem em sua versão mais recente e a atualização agendada é a maneira de fazer isso. Leia mais sobre a "atualização agendada dos relatórios do Power BI no Servidor de Relatórios do Power BI".

### <a name="editing-power-bi-reports-from-the-server"></a>Editando relatórios do Power BI no servidor

É possível abrir e editar os arquivos de relatório do Power BI (.pbix) no servidor, mas você retorna o arquivo original carregado.  Isso significa que **se os dados tiverem sido atualizados pelo servidor, eles não estarão atualizados quando você abrir o arquivo pela primeira vez**. Para ver a alteração, você precisará atualizá-los manual e localmente.

### <a name="large-file-uploaddownload"></a>Upload/download de arquivo grande

Você pode carregar arquivos de até 2 GB, embora, por padrão, esse limite é definido como 1 GB nas configurações do Servidor de Relatórios no SSMS (SQL Server Management Studio).  Esses arquivos são armazenados no banco de dados como no SharePoint e nenhuma configuração especial para o catálogo do SQL Server é necessária.  

### <a name="accessing-shared-datasets-as-odata-feeds"></a>Acessando conjuntos de dados compartilhados como feeds OData

Você pode acessar os conjuntos de dados compartilhados do Power BI Desktop com um feed OData. Para obter mais informações, consulte [Acessando conjuntos de dados compartilhados como feeds OData no Servidor de Relatórios do Power BI](access-dataset-odata.md).

### <a name="scale-out"></a>Escalabilidade horizontal

Esta versão é compatível com escalabilidade horizontal. Use um balanceador de carga e defina a afinidade do servidor para uma melhor experiência. Observe que o cenário ainda não está otimizado para a escalabilidade horizontal, portanto você verá os modelos possivelmente replicados em vários nós. O cenário funcionará sem o balanceador de carga de rede e as sessões temporárias. No entanto, você não só verá um uso excessivo de memória nos nós conforme o modelo for carregado N vezes, mas o desempenho também ficará mais lento entre as conexões conforme o modelo for transmitido a um novo nó entre as solicitações.  

### <a name="administrator-settings"></a>Configurações do administrador

Os administradores podem definir as seguintes propriedades nas Propriedades Avançadas do SSMS para o farm de servidores:

* EnableCustomVisuals: Verdadeiro/Falso
* EnablePowerBIReportEmbeddedModels: Verdadeiro/Falso
* EnablePowerBIReportExportData: Verdadeiro/Falso
* MaxFileSizeMb: agora, o padrão é 1000
* ModelCleanupCycleMinutes: a frequência de verificação para remover modelos da memória
* ModelExpirationMinutes: quanto tempo levará até o modelo expirar e ser removido, com base no último uso
* ScheduleRefreshTimeoutMinutes: quanto tempo pode demorar a atualização de dados para um modelo. Por padrão, duas horas.  Não há nenhum limite máximo.

**Arquivo de configuração rsreportserver.config**

```xml
<Configuration>
  <Service>
    <PollingInterval>10</PollingInterval>
    <IsDataModelRefreshService>false</IsDataModelRefreshService>
    <MaxQueueThreads>0</MaxQueueThreads>
  </Service>
</Configuration>
```

### <a name="developer-api"></a>API para desenvolvedores

A API para desenvolvedores (API REST) apresentada para o SSRS 2017 foi estendida para o Servidor de Relatórios do Power BI trabalhar com arquivos do Excel e .pbix. Um possível caso de uso é, por meio de programação, baixar arquivos do servidor, atualizá-los e publicá-los novamente. Essa é a única maneira de atualizar as pastas de trabalho do Excel com modelos do PowerPivot, por exemplo.

Observe que há uma nova API separada para arquivos grandes, que será atualizada na versão de Servidor de Relatórios do Power BI do Swagger. 

### <a name="sql-server-analysis-services-ssas-and-the-power-bi-report-server-memory-footprint"></a>O SSAS (SQL Server Analysis Services) e o volume de memória do Servidor de Relatórios do Power BI

O Servidor de Relatórios do Power BI agora hospeda o SSAS (SQL Server Analysis Services) internamente. Isso não é específico para a atualização agendada. Hospedar o SSAS pode expandir consideravelmente o volume de memória do servidor de relatório. O arquivo de configuração AS.ini está disponível nos nós do servidor, portanto, se estiver familiarizado com o SSAS, será possível atualizar as configurações, incluindo o limite máximo de memória, o cache de disco, etc. Consulte [Propriedades de servidor do Analysis Services](https://docs.microsoft.com/sql/analysis-services/server-properties/server-properties-in-analysis-services) para obter detalhes.

### <a name="viewing-and-interacting-with-excel-workbooks"></a>Exibição e interação com as pastas de trabalho do Excel

O Excel e o Power BI contêm um portfólio de ferramentas que é exclusivo no setor. Juntas, elas permitem que os analistas de negócios reúnam, moldem, analisem e explorem visualmente seus dados com mais facilidade. Além de exibirem os relatórios do Power BI no portal da Web, os usuários empresariais agora podem fazer o mesmo com as pastas de trabalho do Excel no Servidor de Relatórios do Power BI, o que proporciona a eles uma única localização para publicar e exibir seu conteúdo de autoatendimento do Microsoft BI.

Publicamos um [passo a passo de como adicionar um OOS (Servidor do Office Online) em seu ambiente de versão prévia do Servidor de Relatórios do Power BI](excel-oos.md). Os clientes que têm uma conta de Licenciamento por Volume podem baixar o OOS do Centro de Manutenção da Licença de Volume sem nenhum custo e terão a funcionalidade somente exibição. Uma vez configuradas, os usuários poderão exibir e interagir com as pastas de trabalho do Excel que:

* Não tiverem nenhuma dependência de fonte de dados externa
* Tiverem uma conexão dinâmica com uma fonte de dados externa do SQL Server Analysis Services
* Tiver um modelo de dados PowerPivot

### <a name="support-for-new-table-and-matrix-visuals"></a>Suporte para os novos elementos visuais de matriz e de tabela

O Servidor de Relatórios do Power BI agora é compatível com os novos elementos visuais de matriz e de tabela do Power BI. Para criar relatórios com esses elementos visuais, você precisará de uma versão atualizada do Power BI Desktop para a versão de outubro de 2017. Ela não pode ser instalada lado a lado com a versão do Power BI Desktop (junho de 2017). Para obter a versão mais recente do Power BI Desktop, na [página de download do Servidor de Relatórios do Power BI](https://powerbi.microsoft.com/report-server/), selecione **Opções de download avançadas**.

## <a name="june-2017"></a>Junho de 2017

* Servidor de Relatório do Power BI disponibilizado para o público geral (GA).

## <a name="may-2017"></a>Maio de 2017

* Visualização do Servidor de Relatório do Power BI disponibilizada
* Capacidade de publicar relatórios do Power BI local
  * suporte para visuais personalizados
  * Suporte para **conexões dinâmicas do Analysis Services** somente com as novas fontes de dados que serão fornecidas.
  * Aplicativo Power BI para Celulares atualizado para exibir relatórios do Power BI hospedados no Servidor de Relatório do Power BI
* Colaboração aprimorada em relatórios com comentários

## <a name="next-steps"></a>Próximas etapas

Verifique essas fontes para ficar atualizado sobre os novos recursos no Servidor de Relatórios do Power BI.

* [Blog do Microsoft Power BI](https://powerbi.microsoft.com/blog/)
* [Blog da equipe do SQL Server Reporting Services](https://blogs.msdn.microsoft.com/sqlrsteamblog/)
* O [canal do YouTube Guy in a Cube](https://aka.ms/guyinacube)

Mais perguntas? [Experimente perguntar à Comunidade do Power BI](https://community.powerbi.com/)
