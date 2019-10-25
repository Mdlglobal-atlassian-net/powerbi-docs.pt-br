---
title: Publicar visuais do Power BI no AppSource
description: Saiba como você pode publicar seu visual personalizado no AppSource para que outros possam descobrir e usá-lo.
author: KesemSharabi
ms.author: kesharab
manager: rkarlin
ms.reviewer: ''
ms.service: powerbi
ms.subservice: powerbi-custom-visuals
ms.topic: conceptual
ms.date: 3/27/2019
ms.openlocfilehash: 1841311e94ca593093fa3104b615328927365880
ms.sourcegitcommit: 549401b0e1fad15c3603fe7f14b9494141fbb100
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2019
ms.locfileid: "72307664"
---
# <a name="publish-power-bi-visuals-to-appsource"></a>Publicar visuais do Power BI no AppSource

Saiba como você pode publicar seu visual personalizado no AppSource para que outros possam descobrir e usá-lo.

Depois de criar seu visual personalizado, talvez você queira publicá-lo no AppSource para que outros possam descobrir e usá-lo. Mas, há alguns preparativos que precisam ser feitos antes disso. Para saber mais sobre como criar um visual personalizado, confira Developing a [Power BI Custom Visual](visuals/custom-visual-develop-tutorial.md) (Desenvolvimento de um visual personalizado do Power BI).

   ![Office Store](media/office-store/appsource-01.png)

## <a name="what-is-appsource"></a>O que é o AppSource?

O **AppSource** é o lugar de encontrar aplicativos SaaS e suplementos para seus produtos e serviços da Microsoft. O [AppSource](https://appsource.microsoft.com/marketplace/apps?product=power-bi-visuals) conecta milhões de usuários do Office 365, Dynamics 365, Cortana Intelligence, e outros, a soluções que os ajudam a realizar seu trabalho com mais eficiência, perspicácia ou harmonia do que antes.

## <a name="preparing-to-submit-your-custom-visual"></a>Preparando-se para enviar seu visual personalizado

Após terminar de ler nossas [diretrizes de visuais do Power BI](guidelines-powerbi-visuals.md), programar e [testar seu visual personalizado](https://github.com/Microsoft/PowerBI-visuals/blob/master/Tutorial/SubmissionTesting.md) para empacotá-lo em um arquivo pbiviz, você também deverá preparar o seguinte para envio.

| Item | Necessário | Descrição |
| --- | --- | --- |
| O pacote pbiviz contém todos os metadados necessários |Sim |Nome do visual<br>Nome de exibição<br>GUID<br>Versão<br>Descrição<br>Email e nome do autor |
| Arquivo de relatório .pbix de exemplo |Sim |Para demonstrar seu visual, você deverá ajudar os usuários a se familiarizarem com ele. Você deve enfatizar o valor que o visual traz para o usuário e dar exemplos de uso, opções de formatação, etc. Você também pode adicionar uma página de *"dicas"* no final com algumas dicas e truques, coisas a serem evitadas e assim por diante.<br>O arquivo de relatório .pbix de exemplo deve trabalhar offline, sem nenhuma conexão externa |
| Ícone |Sim |Você deve incluir o logotipo visual personalizado que será exibido na frente da loja. O formato pode ser .png, .jpg, .jpeg ou .gif. Ele deve ter exatamente 300 px (largura) x 300 px (altura). **Importante!** Examine o [guia curto](https://docs.microsoft.com/office/dev/store/craft-effective-appsource-store-images) com atenção antes de enviar o ícone. |
| Capturas de tela |Sim |Você deve fornecer, pelo menos, uma captura de tela. O formato pode ser .png, .jpg, .jpeg ou .gif. Ele deve ter exatamente 1.366 px (largura) x 768 px (altura). Não pode ser maior do que 1.024 KB para o tamanho do arquivo. *Para melhor utilização, adicione bolhas de texto para articular a proposição de valores dos principais recursos mostrados em cada captura de tela.* |
| Link de download de suporte |Sim |Forneça a URL para dar suporte a clientes que têm problemas com seu visual. Esse link é inserido como parte de sua listagem SellerDashboard e fica visível para os usuários quando eles acessam a listagem do seu visual no AppSource. O formato da URL deve incluir https:// ou http://. |
| Link do documento de privacidade |Sim |Forneça um link para a política de privacidade para clientes que usam o visual. Esse link é inserido como parte de sua listagem SellerDashboard e fica visível para os usuários quando eles acessam a listagem do seu visual no AppSource. O formato do link deve incluir https:// ou http://. |
| EULA (Contrato de licença de usuário final) |Sim |Você deve fazer upload de um arquivo EULA. Você pode usar seu próprio EULA ou o EULA padrão na Office store para visuais do Power BI. Para usar o EULA padrão, cole a seguinte URL na caixa de diálogo de upload de arquivo do "Contrato de licença de usuário final" do painel do vendedor: [https://visuals.azureedge.net/app-store/Power BI – Default Custom Visual EULA.pdf](https://visuals.azureedge.net/app-store/Power%20BI%20-%20Default%20Custom%20Visual%20EULA.pdf). |
| Link do vídeo |Não |Para aumentar o interesse dos usuários pelo seu visual personalizado, é recomendável fornecer um link para um vídeo sobre o visual. O formato da URL deve incluir https:// ou http://. |
| Repositório GitHub |Não |É preferível ter um link válido e público para um repositório [GitHub](https://www.github.com) com as fontes do seu visual e dos dados de exemplo nele para permitir que outros desenvolvedores façam comentários e proponham melhorias ao seu código. |

## <a name="submitting-to-power-bi"></a>Envio para o Power BI

O envio é iniciado com um email para a equipe de envio de visuais do Power BI. Você pode enviar um email para [pbivizsubmit@microsoft.com](mailto:pbivizsubmit@microsoft.com).

> [!IMPORTANT]
> Você deve preencher os campos a seguir no arquivo pbiviz.json: "description", "supportUrl", "author", "name" e "email" antes de criar o pacote .pbiviz.

Anexe o **arquivo .pbiviz** e o **exemplo de arquivo .pbix de relatório** em seu email. A equipe do Power BI responderá com instruções e um arquivo XML do pacote do aplicativo para upload. Esse pacote do aplicativo XML é necessário para enviar seu visual por meio da Central de desenvolvedores do Office.

> [!NOTE]
> Para melhorar a qualidade e garantir que os relatórios existentes não sejam danificados, as atualizações para os visuais existentes precisarão de um período adicional de duas semanas para alcançarem o ambiente de produção após a aprovação na loja.

## <a name="submitting-to-appsource"></a>Enviar para AppSource

Depois de obter o XML do pacote do aplicativo da equipe do Power BI, navegue até [central de desenvolvedores](https://sellerdashboard.microsoft.com/Application/Summary) para enviar seu visual ao AppSource.

> [!NOTE]
> Você deve ter uma conta de desenvolvedor do Office válida para efetuar logon na [Central de desenvolvedores do Office](https://dev.office.com/). Uma conta de desenvolvedor do Office deve ser uma Conta da Microsoft (Live ID, por exemplo, hotmail.com ou outlook.com).

> [!IMPORTANT]
> Você deve enviar um email com os arquivos .pbiviz e .pbix para a equipe do Power BI antes de enviar para o AppSource. Isso permite à equipe do Power BI carregar os arquivos para o servidor de compartilhamento público. Caso contrário, a loja não poderá recuperar os arquivos. Você deve enviar os arquivos com cada envio de visual novo, a atualização para o visual existente e as correções para envios rejeitados.

### <a name="process-to-submit-visual"></a>Processo para enviar visual

Siga as etapas abaixo para concluir o envio.

1. Selecione **Adicionar um novo aplicativo**.

    ![Adicionar um aplicativo](media/office-store/powerbi-custom-visual-add-an-app.png)

2. Selecione **Visual personalizado do Power BI** e **Avançar**.

3. Selecione **+** em **Pacote do aplicativo** e selecione o arquivo XML do pacote do aplicativo recebido da equipe do Power BI na caixa de diálogo Abrir Arquivo.

    ![Pacote do aplicativo](media/office-store/powerbi-custom-visual-apppackage.png)

4. Você deve receber uma aprovação de que este é um pacote do aplicativo Power BI válido.

    ![Manifesto aprovado](media/office-store/powerbi-custom-visual-manifest-approved.png)

5. Preencha os detalhes das **Informações gerais**.

   * *Título do envio:* Como seu envio será nomeado na central de desenvolvedores
   * *Versão:* Seu número de versão é preenchido automaticamente no pacote do aplicativo do suplemento.
   * *Data de lançamento (UTC):* Selecione uma data para seu aplicativo ser lançado na loja. Se uma data futura for escolhida, seu aplicativo não estará disponível na loja até essa data.
   * *Categoria:* A primeira categoria será automaticamente preenchida como "Visualização de dados + BI". Esta é a forma como todos os visuais do Power BI serão marcados. Você pode fornecer até duas categorias adicionais para ajudar os usuários a pesquisarem facilmente seu visual
   * *Notas de teste:* opcionais, se você quiser fornecer algumas instruções para os testadores da Microsoft
   * *Meu aplicativo chama, dá suporte para, contém ou usa criptografias:* deixe desmarcado
   * *Tornar este suplemento disponível no catálogo de suplemento do Office no iPad:* deixe desmarcado
6. Faça upload do seu logotipo do visual, selecionando **+** em **Logotipo do aplicativo**. Em seguida, selecione o arquivo de ícone na caixa de diálogo Abrir arquivo. O arquivo deve ser .png, .jpg, .jpeg ou .gif. Ele deve ter exatamente 300 px (largura) x 300 px (altura) e não pode exceder 512 KB de tamanho.

    ![Logotipo do aplicativo](media/office-store/powerbi-custom-visual-app-logo.png)

7. Preencha os detalhes dos **Documentos de suporte**.

   * Link do documento de suporte
   * Link do documento de privacidade
   * Link do vídeo
   * Contrato de Licença de Usuário Final (EULA)

       Você deve fazer upload de um arquivo EULA. Você pode usar seu próprio EULA ou o EULA padrão na Office store para visuais do Power BI. Para usar o EULA padrão, cole a seguinte URL na caixa de diálogo de upload de arquivo do "Contrato de licença de usuário final" do painel do vendedor: [https://visuals.azureedge.net/app-store/Power BI – Default Custom Visual EULA.pdf](https://visuals.azureedge.net/app-store/Power%20BI%20-%20Default%20Custom%20Visual%20EULA.pdf).

8. Selecione **Avançar** para prosseguir para a página **Detalhes**.

9. Selecione **Idioma** e escolha um idioma na lista.

    ![Idioma](media/office-store/powerbi-custom-visual-language.png)

10. Preencha os detalhes da "Descrição".

    * *Nome do aplicativo (para esse idioma):* Insira o título do seu aplicativo, como deve aparecer na vitrine.
    * *Descrição resumida:* Insira uma descrição resumida do seu aplicativo, com até 100 caracteres, como deve aparecer na vitrine. Essa descrição será exibida nas páginas de nível superior, juntamente com o logotipo. Você pode usar a descrição do pacote pbiviz.
    * *Descrição longa:* Forneça uma descrição mais detalhada de seu aplicativo que os clientes verão na sua página de detalhes do aplicativo. Se desejar transformar seu elemento visual em software livre para a comunidade aprimorá-lo, forneça aqui o link para o repositório público, como o GitHub.

11. Faça upload de, pelo menos, uma captura de tela. O formato pode ser .png, .jpg, .jpeg ou .gif. Ele deve ter exatamente 1.366 px (largura) x 768 px (altura). Não pode ser maior do que 1.024 KB para o tamanho do arquivo. *Para melhor utilização, adicione bolhas de texto para articular a proposição de valores dos principais recursos mostrados em cada captura de tela.*

12. Se quiser adicionar mais idiomas, selecione **Adicionar um idioma** e repita as etapas 10 e 11. A adição de mais idiomas ajudará os usuários a exibirem os detalhes visuais personalizados em seu próprio idioma. Os idiomas que não serão listados usarão o primeiro idioma selecionado como padrão.

13. Quando terminar de adicionar os idiomas, selecione **Avançar** para prosseguir para a página **Bloquear o acesso**.

14. Se quiser impedir que clientes em regiões ou países específicos usem ou comprem seu aplicativo, marque a caixa de seleção e escolha na lista.

15. Selecione **Avançar** para prosseguir para a página **Preço**.

16. Atualmente, há suporte apenas para visuais *gratuitos* e aquisições adicionais dentro do visual (compra no aplicativo) não são permitidas. Selecione **Este aplicativo é gratuito**.

    > [!NOTE]
    > Se você selecionar qualquer outra opção que não seja a gratuita ou tiver um conteúdo de compra no aplicativo no visual enviado, o envio será rejeitado.

17. Agora é possível selecionar **Salvar como rascunho** e enviar mais tarde ou selecionar **Enviar para aprovação** para enviar o visual personalizado à Office Store.

## <a name="tracking-submission-status-and-usage"></a>Acompanhamento do uso e do status do envio

Você pode examinar as [políticas de validação](https://dev.office.com/officestore/docs/validation-policies#13-power-bi-custom-visuals).

Após o envio, você poderá exibir o status do envio no [dashboard de aplicativos](https://sellerdashboard.microsoft.com/Application/Summary/).

## <a name="certify-your-visual"></a>Certificar seu visual

Depois de criar seu visual, você tem a opção de certificá-lo. Isso significa que ele pode ser executado no serviço do Power BI e pode ser usado com outros recursos do serviço, como exportar para o PowerPoint. Para obter mais informações, consulte [*Certificando* um visual personalizado](../power-bi-custom-visuals-certified.md).

## <a name="next-steps"></a>Próximas etapas

[Desenvolvimento de um visual personalizado do Power BI](visuals/custom-visual-develop-tutorial.md)  
[Visualizações no Power BI](../visuals/power-bi-report-visualizations.md)  
[Visualizações personalizadas no Power BI](../power-bi-custom-visuals.md)  
[*Certificando* um visual personalizado](../power-bi-custom-visuals-certified.md)

Mais perguntas? [Experimente perguntar à Comunidade do Power BI](http://community.powerbi.com/)
