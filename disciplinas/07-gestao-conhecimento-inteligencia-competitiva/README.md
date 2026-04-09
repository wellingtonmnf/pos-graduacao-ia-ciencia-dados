# 07 · Gestão do Conhecimento e Inteligência Competitiva

> Disciplina do curso de Pós-Graduação em Inteligência Artificial e Ciência de Dados — UNIFACS.

---

## Sobre a disciplina

Inteligência Competitiva é o processo sistemático de coleta, análise e uso de informações sobre o ambiente de negócios para apoiar a tomada de decisão estratégica. Esta disciplina conecta o universo da ciência de dados ao contexto organizacional: dados brutos só geram valor quando transformados em conhecimento acionável. Aqui, o foco está em compreender como organizações criam, gerenciam e sustentam vantagens competitivas a partir de dados — unindo teoria da gestão do conhecimento com técnicas analíticas aplicadas a problemas reais de negócio.

---

## Conteúdo programático

### Fundamentos de inteligência competitiva

- Conceito e histórico de inteligência competitiva
- O ciclo de inteligência: coleta, análise, disseminação e uso
- Diferenças entre dado, informação, comunicação e conhecimento
- Fontes de informação: primárias, secundárias e abertas (OSINT)

### Gestão do conhecimento

- Subsídios teórico-metodológicos sobre gestão do conhecimento
- Conhecimento tácito e explícito
- Modelos de criação e transferência de conhecimento
- Organizações que aprendem

### Vantagens competitivas

- Processos envolvidos na criação e sustentação de vantagens competitivas
- Análise de mercado e monitoramento de concorrentes
- Modelos estratégicos: Porter, SWOT, PESTEL
- Tomada de decisão baseada em dados (data-driven decision making)

---

## Notebooks e materiais

| Material | Tópico | Descrição |
|----------|--------|-----------|
| `01_ciclo_de_inteligencia.ipynb` | Fundamentos | Mapeamento do ciclo de inteligência aplicado a um setor de mercado real |
| `02_analise_de_concorrentes.ipynb` | Competitividade | Coleta e análise automatizada de dados públicos de concorrentes com Python |
| `03_web_scraping_osint.ipynb` | Coleta de dados | Extração de informações de fontes abertas com BeautifulSoup e Scrapy |
| `04_analise_swot_dados.ipynb` | Estratégia | Construção de análise SWOT orientada por dados e visualização dos resultados |
| `05_text_mining_noticias.ipynb` | Monitoramento | Mineração de texto em notícias e relatórios para monitoramento de mercado |
| `06_dashboard_inteligencia.ipynb` | Comunicação | Dashboard de inteligência competitiva para suporte à tomada de decisão |

> Esta disciplina une análise de dados com pensamento estratégico de negócio. Os notebooks cobrem a dimensão técnica; os documentos em `referencias/` aprofundam os modelos teóricos.

---

## Datasets utilizados

| Dataset | Origem | Utilizado em |
|---------|--------|--------------|
| Google Trends (via pytrends) | [Google Trends](https://trends.google.com.br/) | Monitoramento de mercado e concorrentes |
| Yahoo Finance (via yfinance) | [Yahoo Finance](https://finance.yahoo.com/) | Análise competitiva de empresas listadas |
| Common Crawl News | [Common Crawl](https://commoncrawl.org/) | Text mining em notícias |
| Glassdoor / LinkedIn (amostra pública) | Kaggle | Análise de mercado de trabalho e tendências |

> Datasets externos são versionados com [Git LFS](https://git-lfs.com/) e estão na pasta `dados/`.

---

## Referências

### Livros e artigos

- NONAKA, Ikujiro; TAKEUCHI, Hirotaka. **Criação de Conhecimento na Empresa**. Elsevier, 1997. *(obra fundadora da gestão do conhecimento organizacional)*
- PORTER, Michael E. **Vantagem Competitiva**. Campus, 1989. *(referência central em estratégia e competitividade)*
- DAVENPORT, Thomas H.; PRUSAK, Laurence. **Conhecimento Empresarial**. Campus, 1998.
- FULD, Leonard M. **The New Competitor Intelligence**. Wiley, 1994.
- PROVOST, Foster; FAWCETT, Tom. **Data Science para Negócios**. Alta Books, 2016. *(ponte entre ciência de dados e tomada de decisão estratégica)*

### Documentação oficial

- [pytrends](https://pypi.org/project/pytrends/) — API não oficial do Google Trends para Python
- [yfinance](https://pypi.org/project/yfinance/) — Coleta de dados financeiros do Yahoo Finance
- [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/bs4/doc/) — Extração de dados de páginas web
- [Scrapy](https://docs.scrapy.org/en/latest/) — Framework de web scraping para coleta em escala
- [spaCy](https://spacy.io/usage) — Processamento de linguagem natural para mineração de texto
- [Plotly Dash](https://dash.plotly.com/) — Construção de dashboards analíticos interativos

---

## Estrutura de pastas

```
07-gestao-conhecimento-inteligencia-competitiva/
├── notebooks/
│   ├── 01_ciclo_de_inteligencia.ipynb
│   ├── 02_analise_de_concorrentes.ipynb
│   ├── 03_web_scraping_osint.ipynb
│   ├── 04_analise_swot_dados.ipynb
│   ├── 05_text_mining_noticias.ipynb
│   └── 06_dashboard_inteligencia.ipynb
├── dados/
│   ├── raw/
│   └── processed/
├── referencias/
│   └── artigos/
└── README.md
```

---

> [← Voltar ao repositório principal](../../README.md)