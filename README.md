# Azure Cognitive Search

# AI Search com Azure 

Este repositório contém os passos e recursos necessários para completar o **Lab 11** do curso de **Fundamentos de Inteligência Artificial da Microsoft**, focado em **Azure AI Search**. O objetivo deste laboratório é aprender como configurar e utilizar o serviço de pesquisa cognitiva da Azure para indexar e consultar dados com a ajuda de recursos de IA.

## Objetivos

- Criar um **Azure Cognitive Search** para realizar buscas em dados indexados.
- Aprender como usar **Document AI** e **Enrichment** para melhorar a qualidade das buscas.
- Implementar uma solução de pesquisa cognitiva que usa dados textuais para obter insights relevantes.

## Passos para Concluir o Lab

### 1. Criar o Azure AI Search
- Clique em "Criar um recurso"  procure por "Azure Ai Search" e clique em "Criar"
![azure ai service](https://github.com/user-attachments/assets/80680105-c687-4278-ab6d-8643b6e641a6)

- Após clicar em "Criar" você será rediricionado para essa página, selecione o "Grupo de Recursos" (caso não tenha, basta criar um novo) e insira um "Nome do serviço"
![servico pesquisa](https://github.com/user-attachments/assets/9bcece95-61a7-4981-a97e-c152df41f343)

**Não se esqueça de alterar o Tipo de Preço para _Básico_**




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
