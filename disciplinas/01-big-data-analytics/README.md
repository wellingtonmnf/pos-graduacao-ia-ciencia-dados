# 01 · Big Data Analytics

> Disciplina do curso de Pós-Graduação em Inteligência Artificial e Ciência de Dados — UNIFACS.

---

## Sobre a disciplina

Big Data Analytics é o campo dedicado ao armazenamento, processamento e análise de volumes massivos de dados — estruturados, semiestruturados e não estruturados — que ultrapassam a capacidade dos sistemas tradicionais. Esta disciplina cobre desde os fundamentos históricos e conceituais até as tecnologias de infraestrutura, ecossistemas distribuídos e as tendências do mercado de dados, formando a base técnica para atuar como cientista ou engenheiro de dados.

---

## Conteúdo programático

### Fundamentos

- Definição e histórico do Big Data
- Mineração de dados
- Evolução dos modelos de bancos de dados
- Big Data: definição, características (os 5 Vs) e gerenciamento
- Do processo de coleta ao processamento e à geração de conhecimento

### Tipos e tratamento de dados

- Novos tipos de dados: semiestruturados e não estruturados
- Tratamento e gerenciamento de dados massivos

### Infraestrutura e tecnologias

- Tecnologias fundamentais para Big Data: infraestrutura e interfaces
- Desafios estruturais
- Fundamentos do ecossistema Hadoop: MapReduce, Data Lake, HDFS
- Computação em nuvem
- Computação distribuída
- Internet das Coisas (IoT)
- Bancos SQL e NoSQL

### Aplicações e mercado

- Big Data Analytics — técnicas e soluções
- Soluções em Big Data para consumo
- Estudos de caso
- Tendências do mercado
- Cientista de dados: perfil do novo profissional
- Mercado atual e oportunidades

---

## Notebooks

| Notebook | Tópico | Descrição |
|----------|--------|-----------|
| `01_introducao_big_data.ipynb` | Fundamentos | Os 5 Vs do Big Data, histórico e panorama geral do ecossistema |
| `02_hadoop_mapreduce.ipynb` | Infraestrutura | Conceitos de MapReduce e simulação do modelo de processamento distribuído |
| `03_sql_vs_nosql.ipynb` | Bancos de dados | Comparativo prático entre bancos relacionais e NoSQL (MongoDB, Redis) |
| `04_data_lake_pipeline.ipynb` | Arquitetura | Construção de um pipeline simples de ingestão e armazenamento em Data Lake |
| `05_computacao_em_nuvem.ipynb` | Infraestrutura | Introdução aos serviços de nuvem para dados: AWS S3, Google Cloud Storage |
| `06_iot_e_streaming.ipynb` | IoT | Simulação de dados de sensores IoT e processamento em tempo real |
| `07_big_data_analytics.ipynb` | Analytics | Análise exploratória sobre datasets massivos com Pandas e Dask |
| `08_estudo_de_caso.ipynb` | Aplicação | Estudo de caso completo: do dado bruto ao insight |

> Os notebooks seguem a sequência natural da disciplina: fundamentos conceituais → infraestrutura → bancos de dados → pipelines → aplicações analíticas.

---

## Datasets utilizados

| Dataset | Origem | Utilizado em |
|---------|--------|--------------|
| NYC Taxi Trips | [NYC Open Data](https://opendata.cityofnewyork.us/) | Analytics e pipeline |
| IoT Sensor Data | [Kaggle](https://www.kaggle.com/datasets/garystafford/iot-devices) | IoT e streaming |
| Stack Overflow Survey | [Stack Overflow](https://survey.stackoverflow.co/) | SQL vs NoSQL, perfil profissional |
| COVID-19 Open Data | [Google Cloud](https://health.google.com/covid-19/open-data/) | Big Data Analytics |

> Datasets externos são versionados com [Git LFS](https://git-lfs.com/) e estão na pasta `dados/`.

---

## Referências

### Livros e artigos

- MARZ, Nathan; WARREN, James. **Big Data: Principles and Best Practices of Scalable Real-Time Data Systems**. Manning, 2015.
- WHITE, Tom. **Hadoop: The Definitive Guide**. 4. ed. O'Reilly, 2015.
- PROVOST, Foster; FAWCETT, Tom. **Data Science para Negócios**. Alta Books, 2016.
- DEAN, Jeffrey; GHEMAWAT, Sanjay. **MapReduce: Simplified Data Processing on Large Clusters**. Google, 2004. Disponível em: [research.google/pubs/mapreduce-simplified-data-processing-on-large-clusters](https://research.google/pubs/mapreduce-simplified-data-processing-on-large-clusters/)
- GHEMAWAT, Sanjay; GOBIOFF, Howard; LEUNG, Shun-Tak. **The Google File System**. ACM SOSP, 2003. Disponível em: [research.google/pubs/the-google-file-system](https://research.google/pubs/the-google-file-system/)

### Documentação oficial

- [Apache Hadoop](https://hadoop.apache.org/docs/current/) — Documentação oficial do ecossistema Hadoop
- [Apache Spark](https://spark.apache.org/docs/latest/) — Processamento distribuído em memória
- [Apache Kafka](https://kafka.apache.org/documentation/) — Streaming de dados em tempo real
- [MongoDB](https://www.mongodb.com/docs/) — Banco de dados orientado a documentos
- [Dask](https://docs.dask.org/en/stable/) — Computação paralela com interface similar ao Pandas
- [Google Cloud Big Data](https://cloud.google.com/bigquery/docs) — BigQuery e soluções de dados na nuvem
- [AWS Big Data](https://aws.amazon.com/big-data/getting-started/) — Serviços de Big Data na AWS

---

## Estrutura de pastas

```
01-big-data-analytics/
├── notebooks/
│   ├── 01_introducao_big_data.ipynb
│   ├── 02_hadoop_mapreduce.ipynb
│   ├── 03_sql_vs_nosql.ipynb
│   ├── 04_data_lake_pipeline.ipynb
│   ├── 05_computacao_em_nuvem.ipynb
│   ├── 06_iot_e_streaming.ipynb
│   ├── 07_big_data_analytics.ipynb
│   └── 08_estudo_de_caso.ipynb
├── dados/
│   ├── raw/
│   └── processed/
├── referencias/
│   └── artigos/
└── README.md
```

---

> [← Voltar ao repositório principal](../../README.md)