# Pós-Graduação em Inteligência Artificial e Ciência de Dados

![Python](https://img.shields.io/badge/Python-3.10+-blue)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)
![License](https://img.shields.io/badge/License-MIT-green)
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/usuario/pos-graduacao-ia-ciencia-dados/HEAD)
![UNIFACS](https://img.shields.io/badge/UNIFACS-2025--2026-blueviolet)

Repositório dedicado ao armazenamento estruturado de estudos, experimentos e projetos desenvolvidos durante a Pós-Graduação em Inteligência Artificial e Ciência de Dados — UNIFACS. Funciona como laboratório de experimentação e portfólio técnico em IA.

---

## Índice

- [Estrutura do repositório](#estrutura-do-repositório)
- [Disciplinas](#disciplinas)
- [Exemplos de notebooks](#exemplos-de-notebooks)
- [Execução online](#execução-online)
- [Reprodução científica](#reprodução-científica)
- [Tecnologias utilizadas](#tecnologias-utilizadas)
- [Objetivo](#objetivo)

---

## Estrutura do repositório

```
pos-graduacao-ia-ciencia-dados/
├── README.md
├── LICENSE
├── .gitignore
├── requirements.txt
├── environment.yml
├── .gitattributes                          # Git LFS para datasets grandes
│
├── disciplinas/
│   ├── 01-big-data-analytics/
│   │   ├── notebooks/
│   │   ├── dados/
│   │   │   ├── raw/
│   │   │   └── processed/
│   │   ├── referencias/
│   │   └── README.md
│   ├── 02-aprendizado-de-maquina/
│   │   ├── notebooks/
│   │   ├── dados/
│   │   ├── referencias/
│   │   └── README.md
│   ├── 03-engenharia-preparacao-visualizacao-dados/
│   │   ├── notebooks/
│   │   ├── dados/
│   │   ├── referencias/
│   │   └── README.md
│   ├── 04-processamento-dados-massivos-modelos/
│   │   ├── notebooks/
│   │   ├── dados/
│   │   ├── referencias/
│   │   └── README.md
│   ├── 05-processamento-linguagem-natural/
│   │   ├── notebooks/
│   │   ├── dados/
│   │   ├── referencias/
│   │   └── README.md
│   ├── 06-experiencia-usuario-ia/
│   │   ├── notebooks/
│   │   ├── dados/
│   │   ├── referencias/
│   │   └── README.md
│   ├── 07-gestao-conhecimento-inteligencia-competitiva/
│   │   ├── notebooks/
│   │   ├── dados/
│   │   ├── referencias/
│   │   └── README.md
│   └── 08-metodologias-gestao-projetos/
│       ├── notebooks/
│       ├── dados/
│       ├── referencias/
│       └── README.md
│
├── datasets/
│   ├── externos/
│   └── gerados/
│
├── projetos/
│   ├── projeto-01/
│   │   ├── notebooks/
│   │   ├── dados/
│   │   └── README.md
│   └── projeto-final/
│       ├── notebooks/
│       ├── dados/
│       └── README.md
│
├── recursos/
│   ├── imagens/
│   ├── referencias/
│   └── artigos/
│
└── docs/                                   # Jupyter Book → GitHub Pages
    ├── _config.yml
    ├── _toc.yml
    └── intro.md
```

---

## Disciplinas

| # | Disciplina | Conteúdos principais |
|---|------------|----------------------|
| 01 | **Big Data Analytics** | Hadoop, MapReduce, Data Lakes, NoSQL, IoT, computação em nuvem e distribuída |
| 02 | **Aprendizado de Máquina** | Classificação, regressão, redes neurais, deep learning, reinforcement learning |
| 03 | **Engenharia, Preparação e Visualização de Dados** | Qualidade de dados, preparação, visualização, dashboard design |
| 04 | **Processamento de Dados Massivos e Modelos de Aprendizado** | Bancos NoSQL, grafos, SQL, técnicas de agrupamento e regressão |
| 05 | **Processamento de Linguagem Natural** | Tokenização, Bag-of-Words, word2vec, redes neurais recorrentes, LSTM |
| 06 | **Experiência de Usuário e IA** | Design centrado no usuário, comportamento do consumidor, divisão humano-máquina |
| 07 | **Gestão do Conhecimento e Inteligência Competitiva** | Dado → informação → conhecimento, vantagens competitivas |
| 08 | **Metodologias para Gestão de Projetos** | PMBOK, metodologias ágeis, escopo, custo, cronograma, gestão de riscos |

---

## Exemplos de notebooks

| Notebook | Disciplina |
|----------|------------|
| Análise Exploratória de Dados | 03 · Engenharia de Dados |
| Regressão Linear | 02 · Aprendizado de Máquina |
| Bag-of-Words | 05 · NLP |
| Pipeline MapReduce | 01 · Big Data Analytics |
| Clustering K-Means | 04 · Processamento Massivo |
| Rede Neural LSTM | 05 · NLP |

---

## Execução online

### Abrir no Google Colab

Clique em qualquer notebook dentro do repositório e escolha **Open in Colab**.

### Executar com Binder

Clique no badge abaixo para abrir o repositório completo no Binder, sem instalar nada:

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/wellingtonmnf/pos-graduacao-ia-ciencia-dados/HEAD)

```
https://mybinder.org/v2/gh/wellingtonmnf/pos-graduacao-ia-ciencia-dados/HEAD
```

---

## Reprodução científica

```bash
# 1. Clonar o repositório
git clone https://github.com/wellingtonmnf/pos-graduacao-ia-ciencia-dados.git
cd pos-graduacao-ia-ciencia-dados

# 2. Criar ambiente virtual (recomendado)
python -m venv venv
source venv/bin/activate  # Linux/macOS
# venv\Scripts\activate   # Windows

# 3. Instalar dependências
pip install -r requirements.txt

# 4. Executar os notebooks
jupyter notebook
```

> **Datasets grandes** são versionados com [Git Large File Storage (LFS)](https://git-lfs.com/).
> Instale antes de clonar: `git lfs install`

---

## Tecnologias utilizadas

| Categoria | Ferramentas |
|-----------|-------------|
| Linguagem | Python 3.10+ |
| Manipulação de dados | Pandas, NumPy |
| Visualização | Matplotlib, Seaborn |
| Machine Learning | Scikit-learn |
| Deep Learning | TensorFlow, PyTorch |
| Ambiente de desenvolvimento | Jupyter Notebook / JupyterLab |
| Versionamento de dados | Git LFS |
| Documentação | Jupyter Book, GitHub Pages |

---

## Objetivo

Este repositório funciona como:

- **Registro estruturado** do aprendizado ao longo da pós-graduação
- **Laboratório de experimentação** em ciência de dados e inteligência artificial
- **Portfólio técnico navegável** para recrutadores, colaborações e referência pessoal

---

> Pós-Graduação em Inteligência Artificial e Ciência de Dados · UNIFACS · Salvador, BA