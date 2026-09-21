# Projeto CineData Analytics 🚀

Pipeline de Engenharia de Dados desenvolvido para o processamento, transformação e modelagem de dados do ecossistema cinematográfico, utilizando a arquitetura **Medallion (Landing -> Bronze -> Silver -> Gold)** no ambiente Databricks.

---

## Sobre o Projeto

O **CineData Analytics** tem como objetivo centralizar dados brutos relacionados a filmes, bilheterias e avaliações, aplicando processos de limpeza, enriquecimento e agregação para disponibilizar insights analíticos de alta qualidade para consumo de equipes de negócios e GenAI.

---

## Tecnologias Utilizadas

* **Databricks** (Plataforma de Dados Unificada)
* **Apache Spark / PySpark** (Processamento Distribuído)
* **Delta Lake** (Armazenamento confiável e transacional)
* **YAML** (Orquestração de Jobs)

---

## 📁 Estrutura do Repositório

O repositório está organizado da seguinte forma:

```text
CineData-Analytics/
│
├── 📂 Notebooks/
│   ├── Landing_to_Bronze.ipynb         # Ingestão dos dados brutos para a camada Bronze
│   ├── Bronze_to_Silver.ipnyb         # Limpeza, padronização e tipagem para a camada Silver
|   ├── Silver_to_Gold.ipnyb            # Agregações e modelagem analítica para a camada Gold
│   └── Notebook_Visualização.ipnyb      # Notebook onde fiz algumas visualizações dos dados
├── 📂 Job/
│   ├── job.yaml                    # Configuração e definição do Job no Databricks
│   └── execução_job.png            # Evidência da execução bem-sucedida do pipeline no Databricks
│
└── README.md                       # Documentação principal do projeto
```

---

## 🔄 Arquitetura Medallion

1. **Landing / Bronze:** Ingestão dos dados no formato original com adição de metadados de carga.
2. **Silver:** Tratamento de nulos, remoção de duplicatas, padronização de esquemas, etc.
3. **Gold:** Criação de tabelas agregadas e visões de negócio.

---

