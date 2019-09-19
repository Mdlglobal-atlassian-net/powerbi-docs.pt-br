---
title: Parâmetros de URL em relatórios paginados – Construtor de Relatórios do Power BI
description: Este tópico descreve os usos comuns de parâmetros de relatório do Construtor de Relatórios Paginados do Power BI, as propriedades que podem ser definidas, entre outros.
ms.service: powerbi
ms.subservice: report-builder
ms.custom: ''
ms.topic: conceptual
author: maggiesMSFT
ms.author: maggies
ms.reviewer: cfinlan
ms.date: 08/29/2019
ms.openlocfilehash: bda35bfb4690d8109f7bd611e3d319278d235f33
ms.sourcegitcommit: 09ee1b4697aad84d8f4c9421015d7e4dbd3cf25f
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "70302668"
---
# <a name="url-parameters-in-paginated-reports-in-power-bi"></a>Parâmetros de URL em relatórios paginados no Power BI

Você pode enviar comandos para relatórios paginados no Power BI adicionando um parâmetro em uma URL. Por exemplo, você pode ter exibido o relatório usando um conjunto específico de valores de parâmetro de relatório. Você encapsula essas informações na URL usando parâmetros de acesso à URL predefinidos. Você pode personalizar ainda mais a forma como o Power BI processa o relatório inserindo parâmetros para formatos de renderização ou para determinar a aparência e o estilo da barra de ferramentas de relatório. Em seguida, você pode colar essa URL diretamente em um email ou uma página da Web para que outras pessoas experimentem o relatório da mesma maneira em um navegador. 

Aqui estão as ações que você pode executar por meio de parâmetros de acesso à URL: 

- Enviar parâmetros de relatório a um relatório. 
- Iniciar a exportação do conteúdo do relatório em um formato de arquivo compatível. 
- Ocultar ou exibir o painel de parâmetros. 
- Especificar a configuração DeviceInfo. 

Para obter a lista completa de comandos e configurações disponíveis por meio do acesso à URL, confira  [Referência de parâmetro de acesso à URL](#url-access-parameter-reference) mais adiante neste artigo. 

## <a name="url-access-concepts"></a>Conceitos de acesso à URL 

As solicitações de URL para o Power BI contêm parâmetros que são processados pelo serviço. A maneira como o serviço gerencia as solicitações de URL depende dos parâmetros, dos prefixos de parâmetro e dos tipos de itens incluídos na URL. A funcionalidade de URL de relatório paginado é compatível com a maioria dos navegadores e aplicativos que são compatíveis com o endereçamento de URL padrão. 

## <a name="url-access-syntax"></a>Sintaxe do acesso à URL 

As solicitações de URL podem conter vários parâmetros, listados em qualquer ordem. Os parâmetros são separados por um E comercial (&). Os pares de nome e valor são separados por um sinal de igual (=). Por exemplo:

```
powerbiserviceurl?rp:parametervalueh&rdl:parameter=value  
```

## <a name="syntax-description"></a>descrição da sintaxe 

### <a name="powerbiserviceurl"></a>powerbiserviceurl 

A URL do serviço Web do seu locatário do Power BI. Por exemplo: 

**&** Usado para separar pares de nome e valor dos parâmetros de acesso à URL.

**prefixo** Um prefixo para o parâmetro da URL (por exemplo, rp: ou rdl:) que especifique uma ação no Serviço do Power BI. 

> [!NOTE]
> Os parâmetros de relatório exigem um prefixo de parâmetro e diferenciam maiúsculas de minúsculas. 

**parâmetro** O nome do parâmetro. 

### <a name="value"></a>valor 

Texto da URL correspondente ao valor do parâmetro que está sendo usado. 

Para ver exemplos de como passar parâmetros de relatório na URL, confira  [Passar um parâmetro de relatório em uma URL](report-builder-url-pass-parameters.md).

## <a name="url-access-parameter-reference"></a>Referência de parâmetro de acesso à URL

Você pode usar os parâmetros a seguir como parte de uma URL para configurar a aparência e o estilo dos seus relatórios paginados no Power BI. Os parâmetros mais comuns são listados nesta seção. Os parâmetros não diferenciam maiúsculas de minúsculas e começam com o prefixo de parâmetro `rdl:` , se relacionado ao formato de saída.  

### <a name="report-commands-rdl"></a>Comandos de relatório (`rdl:`) 

**Formato de exportação** Especifica o formato no qual renderizar e exportar um relatório. Os valores disponíveis são: 
- PPTX (PowerPoint)
- MHTML 
- IMAGEM 
- EXCELOPENXML (EXCEL) 
- WORDOPENXML (WORD) 
- CSV 
- PDF 
- XML 

## <a name="next-steps"></a>Próximas etapas

- [Passar um parâmetro de relatório em uma URL para um relatório paginado no Power BI](report-builder-url-pass-parameters.md)
- [O que são os relatórios paginados no Power BI Premium?](paginated-reports-report-builder-power-bi.md)