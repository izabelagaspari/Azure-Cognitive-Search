# Azure Cognitive Search

# AI Search com Azure 

Este repositório contém os passos e recursos necessários para completar o **Lab 11** do curso de **Fundamentos de Inteligência Artificial da Microsoft**, focado em **Azure AI Search**. O objetivo deste laboratório é aprender como configurar e utilizar o serviço de pesquisa cognitiva da Azure para indexar e consultar dados com a ajuda de recursos de IA.

## Objetivos

- Criar um **Azure Cognitive Search** para realizar buscas em dados indexados.
- Aprender como usar **Document AI** e **Enrichment** para melhorar a qualidade das buscas.
- Implementar uma solução de pesquisa cognitiva que usa dados textuais para obter insights relevantes.

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
  






 









Primeiro, crie uma instância do **Azure Cognitive Search**. Esse serviço será responsável por criar índices para armazenar e consultar documentos.

1. Acesse o **Azure Portal** e crie um novo recurso de **Azure Cognitive Search**.
2. Defina um nome para o recurso e o grupo de recursos.

### 2. Criar um Container de Blobs no Azure Storage

Os dados a serem indexados precisam estar armazenados em um **Azure Storage Blob**. Crie uma conta de armazenamento no Azure e faça o upload de documentos para um **container de blobs**.

1. Crie uma **Conta de Armazenamento** no Azure.
2. Faça upload de arquivos de dados (como documentos, avaliações de clientes, etc.) para o **container de blobs**.

### 3. Criar o Índice de Pesquisa

Agora, crie um índice no **Azure Cognitive Search** para começar a indexação dos documentos.

1. Defina os campos a serem indexados, como **titulo**, **autor**, **data de criação**, etc.
2. Defina os tipos de dados e os campos pesquisáveis.
3. Inicie a indexação dos documentos.

### 4. Enriquecer os Dados com IA

Use os **Cognitive Skills** do Azure para enriquecer os dados antes de armazená-los no índice. Isso inclui:

- **Extração de Sentimentos**: Identificar sentimentos positivos, negativos ou neutros nos textos.
- **Extração de Phrases-Chave**: Detectar as principais palavras-chave nos documentos.

### 5. Consultar o Índice

Depois que o índice for criado e os dados forem enriquecidos, execute consultas para testar a pesquisa nos dados indexados.

1. Use a API ou o portal de pesquisa para consultar o índice e buscar por termos específicos.
2. Analise os resultados para garantir que as consultas estão retornando os dados corretos.

---

## Tecnologias Utilizadas

- **Azure Cognitive Search**: Para indexação e consulta de dados.
- **Azure Storage**: Para armazenamento de documentos.
- **Azure Cognitive Services**: Para enriquecer dados com IA, como extração de sentimentos e frases-chave.

---

## Conclusão

Esse laboratório ensina como integrar **Azure Cognitive Search** com **Azure Cognitive Services** para criar uma solução de pesquisa cognitiva inteligente. Você aprenderá a configurar e a trabalhar com recursos de IA para melhorar a busca e análise de dados textuais.

---

## Referências

- [Microsoft Learn: Fundamentals of AI](https://microsoftlearning.github.io/mslearn-ai-fundamentals/)
- [Azure Cognitive Search Documentation](https://learn.microsoft.com/en-us/azure/search/)
