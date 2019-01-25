---
title: Log de alterações para o Servidor de Relatório do Power BI
description: Esse log de alterações é para o Servidor de Relatório do Power BI e lista novos itens juntamente com correções de bug para cada build lançado.
author: jtarquino
manager: kfile
ms.reviewer: maggies
ms.service: powerbi
ms.subservice: powerbi-report-server
ms.topic: conceptual
ms.date: 03/31/2018
ms.author: jtarquino
ms.openlocfilehash: 18a2d6833f0013f95ac0a5dea5f1930e5b666dd6
ms.sourcegitcommit: 2c49a7cee9c77f46830ddfa59fdedbf30186d389
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "54488858"
---
# <a name="changelog-for-power-bi-report-server"></a>Log de alterações para o Servidor de Relatório do Power BI

Esse log de alterações é para o Servidor de Relatório do Power BI e lista novos itens juntamente com correções de bug para cada build lançado.

Para obter informações detalhadas sobre os novos recursos, consulte [Novidades no Servidor de Relatório do Power BI](whats-new.md). 

## <a name="january-2019"></a>Janeiro de 2019
- **Servidor de Relatório do Power BI**            
    - *Versão 1.4.6960.38798 (Build 15.0.1102.222), Lançamento: 22 de janeiro de 2019*
        - Recursos
            - Relatórios do Power BI 
                - Suporte para Segurança em Nível de Linha
                - Expandir e recolher nos cabeçalhos de linha de matriz
                - Copiar e colar entre arquivos .pbix
                - Guias de alinhamento inteligente
                - Suporte para Conector SAP BW 2.0
            - Administradores
                - Capacidade de definir extensões de recursos que podem ser carregados para o servidor de relatório
                - Capacidade de restringir os esquemas de hiperlink compatíveis
        - Correções de bug
            - Vulnerabilidade de injeção de HTML
            - A exportação para PDF não está mostrando o símbolo de Euro
            - A ação de salvar uma senha com várias fontes de dados em relatórios do Power BI invalida as senhas não alteradas
            - Visuais exibem problemas no Aplicativo Power BI Mobile depois de ficarem ociosos

- **Power BI Desktop (otimizado para o Servidor de Relatórios do Power BI)**
    - *Versão: 2.65.5313.1421 (janeiro de 2019), lançamento: 22 de janeiro de 2019*
        - Contém as alterações necessárias para conexão com o Servidor de Relatórios do Power BI (janeiro de 2019)  

## <a name="august-2018"></a>Agosto de 2018
- **Servidor de Relatório do Power BI**
    - *Versão 1.3.6816.37243 (Build 15.0.2.557), lançamento: 30 de agosto de 2018*
        - Correções de bug
            - Foi corrigido um problema que ocorria quando o servidor era atualizado de versões anteriores do Servidor de Relatórios de PBI em que um redirecionamento de associação não era atualizado e o cliente via isto:      
            *`
            Failed to load expression host assembly. Details: Could not load file or assembly 'Microsoft.ReportingServices.ProcessingObjectModel, Version=2018.7.0.0, Culture=neutral, PublicKeyToken=89845dcd8080cc91' or one of its dependencies. The located assembly's manifest definition does not match the assembly reference. (Exception from HRESULT: 0x80131040) (rsErrorLoadingExprHostAssembly)
             `*
             
            - O bug de transparência de rótulo de dados agora foi corrigido.
            
    - *Versão 1.3.6801.38816 (Build 15.0.2.540), lançamento: 15 de agosto de 2018*
        - Recursos
            - O suporte para DirectQuery de SSO do SAP HANA com o Kerberos já está disponível para relatórios do Power BI
            - API de visual personalizado fornecida com a versão 1.13.0
            - Os visuais personalizados podem voltar a uma versão anterior compatível com a versão atual da API do servidor (se disponível)

- **Power BI Desktop (otimizado para o Servidor de Relatórios do Power BI)**
    - *Versão: 2.61.5192.641 (agosto de 2018), lançamento: 15 de agosto de 2018*
        - Contém as alterações necessárias para conexão com o Servidor de Relatórios do Power BI (agosto de 2018)         
        
## <a name="march-2018"></a>Março de 2018
- **Servidor de Relatório do Power BI**
    - *Versão 1.2.6690.34729 (Build 15.0.2.402), lançamento: 27 de abril de 2018*
        - Correções de bug
            - Habilitar a migração de catálogos do SQL Server Reporting Services 2017
            - Para relatórios do Power BI (PBIX)
                - Os relatórios podem ser atualizados quando um servidor está configurado para usar a autenticação personalizada
                - Modificar as propriedades de um relatório não redefine as credenciais da fonte de dados
            - Para relatórios paginados (RDL)
                - O uso de funções `Lookup()` ou derivadas, como `LookupSet()` e `MultiLookup()`, em expressões RDL não resultam mais em `#Error`
                - Os relatórios vinculados respeitam o tamanho da página do relatório de destino ao imprimir
                - É possível criar assinaturas para relatórios vinculados que usam parâmetros em cascata
                - É possível alterar padrões de parâmetro com vários valores ao usar o IE11
                - É possível editar as opções de entrega de assinatura controladas por dados
                - É possível exibir e editar assinaturas enquanto a assinatura está em execução
                - Configurar credenciais de fonte de dados não remove as cadeias de caracteres de conexão baseadas em expressão
            - Para KPIs
                - As linhas de tendência são atualizadas com os dados
            - Melhorias na estabilidade geral

    - *Versão 1.2.6660.39920 (Build 15.0.2.389), lançamento: 28 de março de 2018*
        - Correções de bug
            - Para Relatórios do Power BI (PBIX), correção para Exportar Dados que não está funcionando em Visuais do Power BI
            - Para Relatórios do Power BI (PBIX), correção para filtros de URL não estão funcionando
            - Para Relatórios Paginados (RDL), correção para imagens que não são exibidas corretamente no IE11 após a atualização para a versão de março do Servidor de Relatórios do Power BI

    - *Versão 1.2.6648.38132 (Build 15.0.2.378), lançamento: 19 de março de 2018*
        - Atualizações de Segurança
        - Aprimoramentos de acessibilidade
        - Correções de bug
            - Para Relatórios Paginados (RDL), correção de visibilidade de parâmetros em um relatório vinculado que é revertido após a edição de suas propriedades
            - Correção para o portal da Web com autenticação de formulários personalizados que está ignorando o cookie sliding expiration
            - Correção para exportação para o Word, que cria uma altura de linha desigual se o conteúdo da linha está vazio
            - Para Relatórios Paginados (RDL), correção para cadeia de conexão baseada em expressão que é excluída quando alteramos a credencial da fonte de dados
            - Correção para a capacidade de usar um KPI com valores de texto
            - Para Relatórios Paginados (RDL), correção para a capacidade de atribuir um novo conjunto de dados para um Relatório Paginado (RDL) existente
            - Outras correções de estabilidade e de facilidade de uso

- **Power BI Desktop (otimizado para o Servidor de Relatórios do Power BI)**
    - Versão: 2.56.5023.1043 (março de 2018), lançamento: 19 de março de 2018
        - Contém as alterações necessárias para a conexão ao Servidor de Relatórios do Power BI (março de 2018)

## <a name="october-2017"></a>Outubro de 2017

- **Servidor de Relatório do Power BI**
    - *Versão 1.1.6582.41691 (Build 14.0.600.442), lançamento: 10 de janeiro de 2018*
        - Atualizações de Segurança
        - Correções de bug
            - Correção para Model.GetParameters retornando 400
            - Correção para configurar o conjunto de dados compartilhado para Relatórios Paginados existentes (RDL)
            - Correção para ExecutionNotFoundException ao exportar o relatório com valores de parâmetros diferentes para PDF

    - *Versão 1.1.6551.5155 (Build 14.0.600.438), lançamento: 11 de dezembro de 2017*
        - Correções de bug
            - Falha ao salvar dados após a atualização para determinados relatórios do Power BI Desktop.

    - *Versão 1.1.6530.30789 (Build 14.0.600.437), lançamento: 17 de novembro de 2017*
        - Correções de bug
            - Correção para Cenários de Autenticação Básica 
            - A correção para dias da semana não pode ser selecionada na página de agendamentos para Assinaturas, Planos de Atualização de Cache e Instantâneos de Histórico no Portal
            - Para Relatórios Paginados (RDL), correção para expressões na caixa de texto com a propriedade CanGrow configurada como false resulta em valores que não mostram cores e fontes inadequadas
            - Para Relatórios do Power BI (PBIX), a correção para adicionar Legendas de gráfico de linhas renderiza um visual vazio

    - *Versão 1.1.6514.9163 (Build 14.0.600.434), lançamento: 1º de novembro de 2017*
        - Correções de bug
            - Corrigir problemas de confiabilidade de upload para relatórios PBIX acima de 500 MB
            - Corrigir problemas de carregamento de problema para relatórios PBIX acima de 1GB

    - *Versão 1.1.6513.3500 (Build 14.0.600.433), lançamento: 31 de outubro de 2017*
        - Recursos
            - Suporte para modelo de dados inserido
            - Exibição de pasta de trabalho do Excel (com a integração do Servidor do Office Online habilitada)
            - Atualização de dados agendada (PBIX)
            - Suporte para consulta direta
            - Suporte para arquivos grandes (até 2 GB)
            - API REST pública
            - Suporte para conjunto de dados compartilhado no Power BI Desktop (via OData)
            - Suporte para parâmetro de URL para arquivos PBIX
            - Aprimoramentos de acessibilidade

- **Power BI Desktop (otimizado para o Servidor de Relatórios do Power BI)**
    - *Versão: 2.51.4885.3981 (outubro de 2017), lançamento: 10 de abril de 2018*
        - Atualizações de Segurança

    - *Versão: 2.51.4885.2501 (outubro de 2017), lançamento: 10 de janeiro de 2018*
        - Atualizações de Segurança

    - *Versão: 2.51.4885.1423 (outubro de 2017), lançamento: 17 de novembro de 2017*
        - Correções de bug
            - Correção para Power BI Desktop de 32 bits falha na execução em SO x86
            - Para os Relatórios do Power BI (PBIX), correção para mostrar linhas de grade do eixo x
            - Outras correções de bugs secundários

    - *Versão: 2.51.4885.1041 (outubro de 2017), lançamento: 31 de outubro de 2017*
        - Recursos
            - Contém as alterações necessárias para a conexão ao Servidor de Relatórios do Power BI (outubro de 2017)

## <a name="june-2017"></a>Junho de 2017

- **Servidor de Relatório do Power BI**
    - *Build 14.0.600.309, lançamento: 10 de janeiro de 2018*
        - Atualizações de Segurança

    - *Build 14.0.600.305, lançamento: 19 de setembro de 2017*  
        - Correções de bug
            - Atualizar para a versão mais recente do [Controle da Web do Bing Maps](https://msdn.microsoft.com/library/mt712542.aspx)

    - *Build 14.0.600.301, lançamento: 11 de julho de 2017*
        - Correções de bug
            - A marca `{{UserId}}` resolve para as credenciais armazenadas, em vez do usuário que executa o relatório nos Relatórios do Power BI
            - Algumas imagens apresentam falha ao ser renderizadas em relatórios do Servidor de Relatório do Power BI
            - Não é possível alterar o nome de um Relatório do Power BI no Servidor de Relatório do Power BI
            - Não é possível carregar visuais personalizados no aplicativo móvel Power BI (isso requer a reinstalação do aplicativo móvel para limpar o cache local)

    - *Build 14.0.600.271, lançamento: 12 de junho de 2017*
        - Versão inicial do Servidor de Relatório do Power BI

- **Power BI Desktop (otimizado para o Servidor de Relatórios do Power BI)**
    - *Versão: 2.47.4766.4901 (junho de 2017), lançamento: 10 de janeiro de 2018*
        - Atualizações de Segurança

## <a name="next-steps"></a>Próximas etapas

[O que é o Servidor de Relatórios do Power BI?](get-started.md)
[Visão geral do administrador](admin-handbook-overview.md)  
[Instalar o Servidor de Relatório do Power BI](install-report-server.md)  
[Baixar o Construtor de Relatórios](https://www.microsoft.com/download/details.aspx?id=53613)  
[Baixar o SSDT (SQL Server Data Tools)](http://go.microsoft.com/fwlink/?LinkID=616714)

Mais perguntas? [Experimente perguntar à Comunidade do Power BI](https://community.powerbi.com/)
