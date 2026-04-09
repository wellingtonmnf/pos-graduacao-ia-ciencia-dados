# 03 · Engenharia, Preparação e Visualização de Dados

> Disciplina do curso de Pós-Graduação em Inteligência Artificial e Ciência de Dados — UNIFACS.

---

## Sobre a disciplina

Engenharia de Dados é o campo responsável por garantir que os dados cheguem corretos, organizados e prontos para análise ou modelagem. Esta disciplina cobre todo o ciclo de vida do dado: da avaliação de qualidade ao tratamento de inconsistências, passando pelas técnicas de transformação e culminando na comunicação visual dos resultados. Um dado bem preparado é a base de qualquer modelo confiável — e esta disciplina forma exatamente essa competência.

---

## Conteúdo programático

### Qualidade de dados

- Conceitos de qualidade de dados
- Identificação de inconsistências, valores ausentes e outliers
- Métricas e critérios de qualidade

### Tratamento e preparação

- Tratamento e preparação de dados
- Ferramentas e técnicas de processamento de dados
- Limpeza, transformação e normalização

### Visualização da informação

- Fundamentos de visualização da informação
- Arquiteturas de interação
- Métodos e técnicas de organização e visualização de dados
- Dashboard design
- Ferramentas para visualização de dados

---

## Notebooks

| Notebook | Tópico | Descrição |
|----------|--------|-----------|
| `01_qualidade_de_dados.ipynb` | Qualidade | Identificação de valores ausentes, duplicatas, outliers e inconsistências |
| `02_limpeza_e_tratamento.ipynb` | Preparação | Técnicas de limpeza: imputação, remoção, correção de tipos e padronização |
| `03_transformacao_e_normalizacao.ipynb` | Preparação | Normalização, padronização, encoding de variáveis categóricas e feature scaling |
| `04_analise_exploratoria.ipynb` | Exploração | EDA completa: estatísticas descritivas, distribuições e correlações |
| `05_visualizacao_estatica.ipynb` | Visualização | Gráficos com Matplotlib e Seaborn: histogramas, boxplots, heatmaps e scatter plots |
| `06_visualizacao_interativa.ipynb` | Visualização | Gráficos interativos com Plotly e análise dinâmica de dados |
| `07_dashboard_design.ipynb` | Dashboard | Construção de dashboard analítico com Plotly Dash |

> Os notebooks seguem a ordem natural de um projeto de dados real: avaliar qualidade → limpar → transformar → explorar → visualizar → comunicar.

---

## Datasets utilizados

| Dataset | Origem | Utilizado em |
|---------|--------|--------------|
| Titanic | [Kaggle](https://www.kaggle.com/c/titanic) | Limpeza, tratamento e EDA |
| Brazilian E-Commerce (Olist) | [Kaggle](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce) | Visualização e dashboard |
| World Happiness Report | [Kaggle](https://www.kaggle.com/datasets/unsdsn/world-happiness) | Visualização estática e interativa |
| IBGE — Dados Socioeconômicos | [IBGE](https://www.ibge.gov.br/estatisticas/downloads-estatisticas.html) | EDA e visualização geográfica |

> Datasets externos são versionados com [Git LFS](https://git-lfs.com/) e estão na pasta `dados/`.

---

## Referências

### Livros e artigos

- WICKHAM, Hadley; GROLEMUND, Garrett. **R for Data Science**. O'Reilly, 2017. Disponível em: [r4ds.had.co.nz](https://r4ds.had.co.nz/) *(os conceitos de tidy data se aplicam diretamente ao Python)*
- WILKE, Claus O. **Fundamentals of Data Visualization**. O'Reilly, 2019. Disponível em: [clauswilke.com/dataviz](https://clauswilke.com/dataviz/)
- KNAFLIC, Cole Nussbaumer. **Storytelling com Dados**. Alta Books, 2019.
- WICKHAM, Hadley. **Tidy Data**. Journal of Statistical Software, 2014. Disponível em: [jstatsoft.org/article/view/v059i10](https://www.jstatsoft.org/article/view/v059i10)
- DASU, Tamraparni; JOHNSON, Theodore. **Exploratory Data Mining and Data Cleaning**. Wiley, 2003.

### Documentação oficial

- [Pandas](https://pandas.pydata.org/docs/user_guide/index.html) — Manipulação e preparação de dados tabulares
- [NumPy](https://numpy.org/doc/stable/user/index.html) — Computação numérica e operações em arrays
- [Matplotlib](https://matplotlib.org/stable/users/index.html) — Visualização estática de dados
- [Seaborn](https://seaborn.pydata.org/tutorial.html) — Visualização estatística de alto nível
- [Plotly](https://plotly.com/python/) — Gráficos interativos em Python
- [Plotly Dash](https://dash.plotly.com/) — Construção de dashboards analíticos
- [Scikit-learn: Preprocessing](https://scikit-learn.org/stable/modules/preprocessing.html) — Normalização, encoding e transformações

---

## Estrutura de pastas

```
03-engenharia-preparacao-visualizacao-dados/
├── notebooks/
│   ├── 01_qualidade_de_dados.ipynb
│   ├── 02_limpeza_e_tratamento.ipynb
│   ├── 03_transformacao_e_normalizacao.ipynb
│   ├── 04_analise_exploratoria.ipynb
│   ├── 05_visualizacao_estatica.ipynb
│   ├── 06_visualizacao_interativa.ipynb
│   └── 07_dashboard_design.ipynb
├── dados/
│   ├── raw/
│   └── processed/
├── referencias/
│   └── artigos/
└── README.md
```

---

> [← Voltar ao repositório principal](../../README.md)