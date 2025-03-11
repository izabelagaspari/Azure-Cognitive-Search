# Azure Cognitive Search

## O que é o Azure Cognitive Search?

O *Azure Cognitive Search* é um serviço de busca na nuvem altamente escalável e completo, oferecido pela Microsoft Azure. Ele permite que você adicione funcionalidades de pesquisa poderosas em seus aplicativos e soluções, com o suporte de ferramentas de inteligência artificial (IA) para melhorar a relevância e os resultados de busca.

O serviço combina a pesquisa tradicional com capacidades cognitivas avançadas, como análise de texto, reconhecimento de imagem e processamento de linguagem natural, para proporcionar uma experiência de busca rica e eficiente.

## Principais Funcionalidades

- *Pesquisa Inteligente*: Azure Cognitive Search fornece uma pesquisa de texto completo, com suporte para filtros, facetas, e sugestões, tornando a busca mais relevante e precisa.
  
- *Análise de Texto*: O serviço usa o processamento de linguagem natural (PNL) para extrair informações importantes de dados não estruturados, como textos, documentos e páginas da web.

- *Indexação de Dados*: Com o Azure Cognitive Search, você pode indexar uma variedade de dados, incluindo documentos, bancos de dados e imagens, tornando a busca mais rápida e precisa.

- *Integração com Serviços Cognitivos*: O serviço pode ser integrado com APIs do Azure Cognitive Services, como **Computer Vision* e *Text Analytics*, para realizar tarefas de extração de texto a partir de imagens, detecção de sentimentos, e muito mais.

- *Escalabilidade*: Azure Cognitive Search pode escalar automaticamente conforme a demanda de sua aplicação, garantindo alta disponibilidade e desempenho.

## Casos de Uso Comuns

- *Sistemas de E-commerce*: Implementação de funcionalidades de pesquisa avançada para produtos, filtragem por categorias, e sugestões de produtos relacionadas.
  
- *Documentos e Conteúdo*: Indexação de grandes volumes de documentos (como .pdf, .docx, .txt) para permitir a pesquisa de informações em tempo real.

- *Empresas de Mídia e Imagem*: Extração e indexação de dados de imagens para facilitar a busca por imagens relevantes em grandes repositórios.

- *Automação e Inteligência Artificial*: Melhoria da busca utilizando IA, como análise de sentimentos em feedbacks de clientes ou classificações automáticas de documentos.

## Como Funciona?

1. *Criação do Índice*: O primeiro passo é criar um índice, que é uma estrutura que armazena os dados que você deseja pesquisar.
   
2. *Indexação de Dados*: Após criar o índice, você pode começar a indexar os dados. Isso inclui importar dados de várias fontes e garantir que o conteúdo seja processado de forma eficaz para otimizar a busca.

3. *Consultas de Pesquisa*: Depois de indexados, os dados ficam disponíveis para consultas de pesquisa. Você pode aplicar filtros, facetas e até mesmo personalizar os resultados com base na relevância.

4. *Pesquisa Cognitiva*: Para ir além da pesquisa tradicional, você pode integrar o serviço com APIs cognitivas do Azure para análise de texto, tradução de idiomas, e até reconhecimento de entidades dentro de textos.

## Vantagens do Azure Cognitive Search

- *Facilidade de Implementação*: Você pode começar a utilizar o Azure Cognitive Search com pouca configuração e integração mínima com seus aplicativos.
  
- *Escalabilidade e Alta Disponibilidade*: O serviço é gerido pela Microsoft, garantindo alta disponibilidade e capacidade de escalar conforme necessário.

- *Integração com Outros Serviços do Azure*: Ele se integra de forma nativa com outros serviços do Azure, como Azure Blob Storage, Azure SQL Database, e Azure Cognitive Services.

- *Customização Avançada*: Oferece várias opções para customizar e melhorar os resultados da busca, incluindo personalização de relevância e análise semântica.

# AI Search e AI Service com Azure 

Este repositório contém os passos e recursos necessários para completar o **Lab 11** do curso de **Fundamentos de Inteligência Artificial da Microsoft**, focado em **Azure AI Search** e **Azure AI Services**. O objetivo deste laboratório é aprender como configurar e utilizar o serviço de pesquisa cognitiva da Azure para indexar e consultar dados com a ajuda de recursos de IA.

## Objetivos

- Criar um **Azure Cognitive Search** para realizar buscas em dados indexados.
- Aprender como usar **Document AI** e **Enrichment** para melhorar a qualidade das buscas.
- Implementar uma solução de pesquisa cognitiva que usa dados textuais para obter insights relevantes.

## Tecnologias Utilizadas

- **Azure Cognitive Search**: Para indexação e consulta de dados.
- **Azure Storage**: Para armazenamento de documentos.
- **Azure Cognitive Services**: Para enriquecer dados com IA, como extração de sentimentos e frases-chave.
  
---

## Passos para Concluir o Lab

### 1. Criar o Azure AI Search

#### 1. Criar um recurso 
- Na página inicial do Azure, clique em "Criar um recurso"
![criar recurso](https://github.com/user-attachments/assets/0ba8f046-475a-45d1-84ff-c032a3a89ade)

#### 2. Procurar por "Azure AI Search"
- Clique em "Criar"
![azure ai service](https://github.com/user-attachments/assets/80680105-c687-4278-ab6d-8643b6e641a6)

#### 3. Configuração do Serviço
- Após clicar em "Criar", você será redirecionado para a página de configuração do serviço.
- Selecione o "Grupo de Recursos" (caso não tenha, crie um novo)
- Insira um "Nome do Serviço" e altere o "Tipo de Preço" para **Básico**.
- Clique em "Revisar e + criar".
![servico pesquisa](https://github.com/user-attachments/assets/b834c834-1677-42a3-83fc-4211ce3ddb0b)

#### 4. Finalizar a Criação
- Na próxima tela, revise as configurações e clique em "Criar".
 ![criar](https://github.com/user-attachments/assets/dad1288b-9e6c-4537-b7c5-885ee96c52bf)

#### 5. Conclusão
- O processo de criação será iniciado, e ao concluir, você verá a tela de sucesso.
![tudo ok](https://github.com/user-attachments/assets/09b9b5eb-cdab-4f5b-be1f-21faff070804)

**Conclusão da criação do Azure AI Search!!**

---

## 2. Criar o Azure AI Services

#### 1. Sair do Azure AI Search
- Clique em "Página Inicial" para sair do Azure AI Search e retornar à página principal do Azure.
- Em seguida, clique novamente em "Criar um recurso".
![criar recurso](https://github.com/user-attachments/assets/0ba8f046-475a-45d1-84ff-c032a3a89ade)

#### 2. Procurar por "Azure AI Services"
- Procure por "Azure Ai services" e clique em "Criar"
![service](https://github.com/user-attachments/assets/0a5766f2-ee23-4385-a588-c762fbd0ce06)

#### 3. Configuração do Serviço
- Escolha o mesmo "Grupo de Recursos" da Azure AI Search, insira um "Nome" e escolha o "Tipo de preço". 
- **Não esqueça de marcar a checkbox dos termos**.
- Clique em "Examinar + criar"
![servico cognitivo](https://github.com/user-attachments/assets/c980e35c-2eae-4f70-bde0-7d809eebcbd1)

#### 4. Finalizar a Criação
- Após revisar as configurações, clique em "Criar" e aguarde o processo de criação ser concluído.
![criar services](https://github.com/user-attachments/assets/75d3e226-e469-4a91-a34d-ab1332cbebae)

#### 5. Conclusão
- Após alguns segundos, a criação do serviço será concluída, e a tela de sucesso será exibida.
![td ok](https://github.com/user-attachments/assets/a7eb0651-74d1-4eee-91ae-2d9a387efe98)

**Conclusão da criação da Azure AI Services!!**


---
## 3. Criar Storage Account

#### 1. Sair do Azure AI Services
- Clique em "Página Inicial" para sair do Azure AI Services e retornar à página principal do Azure.
- Na barra de pesquisa, digite "Storage Account" e selecione a opção correspondente.
![storage account](https://github.com/user-attachments/assets/ed877cb2-b6d9-4e62-9b6e-d497174e18eb)

#### 2. Criar Storage Account
- Clique em "+ Criar" para iniciar o processo de criação do Storage Account.
![criar sa](https://github.com/user-attachments/assets/22f5a4f3-3a04-468f-bd23-e82fa9c4f97b)

#### 3. Configuração do Serviço
- Preencha as seguintes informações na tela de configuração:
  - Nome da Conta de Armazenamento: Escolha um nome único para a sua conta.
  - Serviço Primário: Selecione "Armazenamento de Blobs do Azure...".
  - Desempenho: Escolha "Standard".
  - Redundância: Selecione "LRS" (Redundância Local).
- Após preencher os campos, clique em "Examinar + Criar".
![detalhes](https://github.com/user-attachments/assets/432eefa2-07f4-4fc6-a54d-1d0c624e2d68)

#### 4. Finalizar a Criação
- Revise as configurações e clique em "Criar".
- Aguarde enquanto o Azure cria a sua conta de armazenamento.
![criar sa 2](https://github.com/user-attachments/assets/f6fc0379-1da9-4531-ad91-26deb50b7cb5)

#### 5. Conclusão da Criação 
- Após alguns segundos, a criação do serviço será concluída. Clique em "Ir para o recurso" para acessar sua conta de armazenamento.
![td ok 2](https://github.com/user-attachments/assets/0a50d0b9-46e5-4e04-a5ab-8a014728387a)

#### 6. Configuração da Conta de Armazenamento
- Na página do recurso, clique em "Configuração".
![configuracao](https://github.com/user-attachments/assets/16d980cf-2340-4ac1-bbdc-07902fbcd7f0)

#### 7. Habilitar Acesso ao Blob
- Na página de configuração, localize a opção "Permitir acesso anônimo ao Blob".
- Clique em "Habilitado" para ativar o acesso anônimo.
- Clique em "Salvar" para confirmar a alteração
![blob](https://github.com/user-attachments/assets/1d4dd199-f8cb-440e-b549-e45043a0b5f8)

#### 8. Criar Contêiner
- Vá para a seção "Contêineres" e clique em "+ Contêiner" para criar um novo contêiner.
- Preencha as seguintes opções:
  - Nome: Escolha um nome para o contêiner.
  - Nível de Acesso Anônimo: Selecione "Contêiner (acesso de leitura)".
- Clique em "Criar" para criar o contêiner.
![conteiner](https://github.com/user-attachments/assets/0d172ffd-3118-4b2b-86a1-a6ba21620144)

#### 9. Contêineres
- Clique no contêiner recém-criado para acessar suas configurações.
- Clique em "Carregar" para adicionar os arquivos que serão analisados.
- Selecione o contêiner criado anteriomente.
![carregar arquivos](https://github.com/user-attachments/assets/f4374dc8-0a43-4e37-9e96-216f66a4e61e)

 **Conclusão da criação da Service Account!!**

---

 ## 4 Impotando dados para o AI Search

 #### 1. Sair do Service Account
- Clique em "Página Inicial" para sair do Service Account e retornar à página principal do Azure.
- Procure pelo arquivo que você criou no AI Service e clique nele.
![ai search](https://github.com/user-attachments/assets/46799258-bc0a-46a4-8b72-41ac2e76c082)

 #### 2. Importar dados
 - Clique na opção "Importar dados"
![importar dados](https://github.com/user-attachments/assets/cdbfe69b-9b38-40f3-bcf6-9dce95d4b9f5)

 #### 3. Importar dados
 - Na página de importar dados sera exibida o Storage Account (caso tenha os arquivos), selecione.
 - Clique em "Próximo: Adicionar habilidades cognitivas"


 #### 4. Explorador de pesquisa
 - Volte para o AI Search e clique em "Explorador de pesquisa"
 ![explorador](https://github.com/user-attachments/assets/1c1816e5-9aa1-46a1-a86c-68659bb9c3b7)
  

---

## Conclusão

Esse laboratório ensina como integrar **Azure Cognitive Search** com **Azure Cognitive Services** para criar uma solução de pesquisa cognitiva inteligente. Você aprenderá a configurar e a trabalhar com recursos de IA para melhorar a busca e análise de dados textuais.

---

## Referências

- [Microsoft Learn: Fundamentals of AI](https://microsoftlearning.github.io/mslearn-ai-fundamentals/)
- [Azure Cognitive Search Documentation](https://learn.microsoft.com/en-us/azure/search/)
