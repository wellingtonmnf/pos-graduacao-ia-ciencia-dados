# 04 · Processamento de Dados Massivos e Modelos de Aprendizado

> Disciplina do curso de Pós-Graduação em Inteligência Artificial e Ciência de Dados — UNIFACS.

---

## Sobre a disciplina

Processamento de Dados Massivos é o campo que une infraestrutura de armazenamento em escala com técnicas de aprendizado de máquina aplicadas diretamente sobre grandes volumes de dados. Esta disciplina cobre desde a modelagem relacional e não relacional de bancos de dados até a aplicação de algoritmos de IA — como deep learning, sistemas de recomendação e técnicas de agrupamento e regressão — sobre bases massivas, integrando o domínio de engenharia de dados com o de ciência de dados.

---

## Conteúdo programático

### Armazenamento massivo

- Armazenamento massivo de dados
- Bancos orientados a documento e grafos
- Modelagem relacional para bancos de dados
- Definição das regras de acesso

### SQL e consultas relacionais

- Formulação de consultas SQL
- Modelagem e implementação de bases relacionais

### Bancos não relacionais

- Modelagem e implementação com modelos não relacionais
- Bases NoSQL: documento, chave-valor, colunar e grafos

### Modelos de Aprendizado sobre dados massivos

- Introdução à Inteligência Artificial aplicada a grandes volumes
- Deep Learning em escala
- Sistemas de recomendação
- Técnicas de Aprendizagem de Máquinas
- Análise de Dados baseada em Estatística
- Técnicas de agrupamento
- Técnicas de regressão

---

## Notebooks

| Notebook | Tópico | Descrição |
|----------|--------|-----------|
| `01_modelagem_relacional.ipynb` | SQL | Modelagem de banco relacional, criação de tabelas e definição de regras de acesso |
| `02_consultas_sql_avancadas.ipynb` | SQL | JOINs, subqueries, agregações e otimização de consultas |
| `03_nosql_documentos.ipynb` | NoSQL | Modelagem e consultas no MongoDB com PyMongo |
| `04_nosql_grafos.ipynb` | NoSQL | Modelagem de grafos com Neo4j e consultas em Cypher |
| `05_processamento_spark.ipynb` | Escala | Processamento distribuído de dados massivos com Apache Spark e PySpark |
| `06_deep_learning_escala.ipynb` | Deep Learning | Treinamento de redes neurais sobre grandes volumes com TensorFlow e GPU |
| `07_sistema_de_recomendacao.ipynb` | Recomendação | Filtragem colaborativa e baseada em conteúdo com Surprise e Scikit-learn |
| `08_agrupamento_e_regressao.ipynb` | ML | Técnicas de clustering e regressão aplicadas a datasets massivos com Dask |

> Os notebooks transitam entre os dois eixos da disciplina: infraestrutura de dados (SQL, NoSQL, escala) e modelos de aprendizado aplicados sobre esses dados.

---

## Datasets utilizados

| Dataset | Origem | Utilizado em |
|---------|--------|--------------|
| Northwind Database | [GitHub](https://github.com/pthom/northwind_psql) | Modelagem relacional e SQL |
| MovieLens | [GroupLens](https://grouplens.org/datasets/movielens/) | Sistema de recomendação |
| Yelp Open Dataset | [Yelp](https://www.yelp.com/dataset) | NoSQL (documentos) e análise massiva |
| Brazilian E-Commerce (Olist) | [Kaggle](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce) | SQL avançado e agrupamento |

> Datasets externos são versionados com [Git LFS](https://git-lfs.com/) e estão na pasta `dados/`.

---

## Referências

### Livros e artigos

- KLEPPMANN, Martin. **Designing Data-Intensive Applications**. O'Reilly, 2017. *(referência central da disciplina — cobre bancos relacionais, NoSQL, replicação e processamento distribuído)*
- SADALAGE, Pramod J.; FOWLER, Martin. **NoSQL Distilled**. Addison-Wesley, 2012.
- CHAMBERS, Bill; ZAHARIA, Matei. **Spark: The Definitive Guide**. O'Reilly, 2018. Disponível em: [pages.databricks.com/rs/094-YMS-629/images/LearningSpark2.0.pdf](https://pages.databricks.com/rs/094-YMS-629/images/LearningSpark2.0.pdf)
- AGGARWAL, Charu C. **Recommender Systems: The Textbook**. Springer, 2016.
- CODD, E. F. **A Relational Model of Data for Large Shared Data Banks**. ACM, 1970. *(artigo original que fundou os bancos relacionais)*

### Documentação oficial

- [PostgreSQL](https://www.postgresql.org/docs/) — Banco relacional robusto e open source
- [MongoDB](https://www.mongodb.com/docs/) — Banco orientado a documentos
- [Neo4j](https://neo4j.com/docs/) — Banco de dados de grafos
- [Apache Spark / PySpark](https://spark.apache.org/docs/latest/api/python/) — Processamento distribuído em Python
- [Dask](https://docs.dask.org/en/stable/) — Computação paralela com interface similar ao Pandas
- [Surprise](https://surpriselib.com/) — Biblioteca Python para sistemas de recomendação
- [SQLAlchemy](https://docs.sqlalchemy.org/) — ORM e toolkit SQL para Python

---

## Estrutura de pastas

```
04-processamento-dados-massivos-modelos/
├── notebooks/
│   ├── 01_modelagem_relacional.ipynb
│   ├── 02_consultas_sql_avancadas.ipynb
│   ├── 03_nosql_documentos.ipynb
│   ├── 04_nosql_grafos.ipynb
│   ├── 05_processamento_spark.ipynb
│   ├── 06_deep_learning_escala.ipynb
│   ├── 07_sistema_de_recomendacao.ipynb
│   └── 08_agrupamento_e_regressao.ipynb
├── dados/
│   ├── raw/
│   └── processed/
├── referencias/
│   └── artigos/
└── README.md
```

---

> [← Voltar ao repositório principal](../../README.md)