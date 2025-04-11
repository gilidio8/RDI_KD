# Metodologia

## Visão Geral

O projeto StackOverLord tem como objetivo criar um sistema inteligente que recomenda trechos de código comentados com base em incidentes e histórico de commits. Para isso, utiliza Inteligência Artificial, modelos de linguagem (LLMs), análise de similaridade e feedback contínuo dos usuários.

A seguir, é apresentada a metodologia detalhada com os componentes necessários, tecnologias recomendadas e arquitetura geral do sistema.

---

## 1. Arquitetura do Sistema

### Componentes Principais

- **Coleta de Dados**: integração com plataformas como Jira, Zendesk, GitHub/GitLab.
- **Armazenamento**: banco de dados relacional + banco vetorial.
- **IA e Recomendação**: uso de LLMs e embeddings.
- **Interface Conversacional**: chatbot ou frontend de busca.
- **Aprendizado Contínuo**: coleta de feedback e reindexação.

---

## 2. Treinamento da IA

### Abordagem Recomendada

#### a) Uso de LLMs com Fine-Tuning ou Similaridade Vetorial

- **LLMs Pré-treinadas**: utilizar modelos como GPT-4, CodeBERT, Starcoder, ou Phi.
- **Fine-tuning (opcional)**: com técnicas leves como LoRA ou Prompt-tuning.
- **Embeddings**: gerar vetores de representações semânticas de trechos e perguntas.

📚 **Bibliotecas sugeridas**:
- `transformers` (HuggingFace)
- `peft` (Parameter-Efficient Fine-Tuning)
- `sentence-transformers`
- `langchain` ou `llama-index`

---

## 3. Banco de Dados

### Necessidades

- Armazenar registros de incidentes
- Armazenar histórico de commits
- Guardar trechos de código + comentários
- Indexar embeddings vetoriais
- Armazenar feedback dos usuários

### Soluções Recomendadas

| Tipo                     | Tecnologia                  |
|--------------------------|-----------------------------|
| Banco Relacional         | PostgreSQL + pgvector       |
| Banco Vetorial           | Faiss, Elasticsearch, Weaviate |
| Busca Full-text          | Elasticsearch               |

---

## 4. Coleta e Pré-processamento dos Commits

### Etapas

1. **Extração**
   - Via GitPython (repositórios locais)
   - Via API GitHub/GitLab

2. **Parsing**
   - Separar código, comentários e mensagens de commit
   - Relacionar com arquivos alterados e datas

3. **Pré-processamento**
   - Limpeza textual
   - Normalização e tokenização
   - Geração de embeddings

📚 Bibliotecas úteis:
- `GitPython`
- `re` (regex), `nltk`, `spacy` para NLP básico
- `sentence-transformers` para embeddings

---

## 5. Mecanismo de Recomendação

### Fluxo

1. **Entrada do Usuário**
   - Via interface de busca ou chatbot
2. **Geração de Embedding**
   - Texto da pergunta é vetorizado
3. **Busca por Similaridade**
   - Faiss / Elasticsearch compara com base de código indexada
4. **Retorno**
   - Sugestões mais relevantes são exibidas

---

## 6. Aprendizado Contínuo

### Feedback Loop

- Usuário marca sugestões como úteis ou não
- Dados de feedback são armazenados
- Nova indexação ou reordenação é feita
- (Opcional) Ajuste leve de parâmetros do modelo

---

## 7. Avaliação de Desempenho

### Métricas

| Métrica      | Função                                                |
|--------------|--------------------------------------------------------|
| **RMSE**     | Mede erro quadrático médio entre sugestões e solução  |
| **MAE**      | Mede o erro absoluto médio                            |
| **Precision@k** | Avalia se as sugestões do top-k foram relevantes     |

📚 Ferramentas:
- `scikit-learn`
- `numpy`, `pandas`

---

## 8. Tecnologias Recomendadas

| Finalidade                    | Ferramenta/Biblioteca                      |
|-------------------------------|--------------------------------------------|
| Modelos de linguagem (LLM)    | OpenAI, HuggingFace, Mistral, LLaMA        |
| Embeddings                    | `sentence-transformers`, `transformers`    |
| Banco vetorial                | Faiss, Elasticsearch, Weaviate             |
| Banco relacional              | PostgreSQL (com extensão `pgvector`)       |
| Coleta de commits             | GitPython, APIs GitHub/GitLab              |
| Avaliação de modelos          | `scikit-learn`, `numpy`                    |
| Frontend / UI                 | Streamlit, React, Gradio                   |
| Integração com IA             | LangChain, LlamaIndex                      |

---

## 9. Considerações Finais

A arquitetura proposta combina tecnologias de ponta com metodologias práticas para garantir alta performance, escalabilidade e facilidade de uso. O projeto permite evoluções futuras, como recomendação de soluções em tempo real, integração com ferramentas CI/CD, e até mesmo automação de respostas a incidentes.

