# 08 · Metodologias para Gestão de Projetos

> Disciplina do curso de Pós-Graduação em Inteligência Artificial e Ciência de Dados — UNIFACS.

---

## Sobre a disciplina

Gestão de Projetos é a disciplina que conecta o conhecimento técnico em IA e Ciência de Dados à capacidade de entregar soluções no mundo real — dentro do prazo, do orçamento e com a qualidade esperada. Projetos de dados têm características únicas: escopo incerto, resultados probabilísticos e ciclos de experimentação contínuos. Esta disciplina forma a competência de escolher e aplicar a metodologia certa para cada contexto, liderar times multidisciplinares e conduzir projetos de IA do planejamento ao encerramento com consistência e clareza.

---

## Conteúdo programático

### Fundamentos de gerência de projetos

- Apresentação de gerência de projetos
- Papel do líder e do time do projeto
- Metodologias e ciclo de vida de gestão de projetos
- Projetos de dados e IA: particularidades e desafios

### Boas práticas e frameworks

- Boas práticas de gerência apresentadas no PMBOK pelo PMI
- As dez áreas de conhecimento do PMBOK
- Grupos de processos: iniciação, planejamento, execução, monitoramento e encerramento

### Metodologias ágeis

- Metodologia ágil: princípios e valores
- Scrum: papéis, cerimônias e artefatos
- Kanban: fluxo e gestão visual
- Critérios para escolha da metodologia a depender do tipo de projeto

### Planejamento e controle

- Técnicas para iniciação e planejamento de projetos
- Definição de escopo, custo e cronograma
- Gestão de riscos
- Métodos para executar, monitorar e controlar projetos
- Ferramentas para encerramento de projetos

---

## Notebooks e materiais

| Material | Tópico | Descrição |
|----------|--------|-----------|
| `01_estrutura_wbs.ipynb` | Planejamento | Construção de EAP (Estrutura Analítica do Projeto) para um projeto de IA com visualização em Python |
| `02_cronograma_gantt.ipynb` | Planejamento | Criação e visualização de cronograma em gráfico de Gantt com Plotly |
| `03_gestao_de_riscos.ipynb` | Riscos | Matriz de probabilidade e impacto, priorização e plano de resposta a riscos |
| `04_metricas_ageis.ipynb` | Ágil | Análise de métricas de times ágeis: velocity, burndown chart e cycle time |
| `05_kanban_simulacao.ipynb` | Ágil | Simulação de fluxo Kanban e identificação de gargalos com dados reais de um projeto |
| `06_encerramento_licoes.ipynb` | Encerramento | Template de registro de lições aprendidas e relatório de encerramento de projeto |

> Esta disciplina tem forte componente prático e documental. Os notebooks focam em ferramentas quantitativas de gestão; os documentos em `referencias/` cobrem os frameworks teóricos completos.

---

## Datasets utilizados

| Dataset | Origem | Utilizado em |
|---------|--------|--------------|
| GitHub Issues (via API) | [GitHub REST API](https://docs.github.com/en/rest) | Métricas ágeis e análise de fluxo |
| Jira Export (CSV simulado) | Gerado | Burndown chart e velocity de sprints |
| Project Management Dataset | [Kaggle](https://www.kaggle.com/datasets/zsinghrahulk/project-management-dataset) | Gestão de riscos e cronograma |

> Datasets externos são versionados com [Git LFS](https://git-lfs.com/) e estão na pasta `dados/`.

---

## Referências

### Livros e artigos

- PROJECT MANAGEMENT INSTITUTE. **Guia PMBOK — Um Guia do Conhecimento em Gerenciamento de Projetos**. 7. ed. PMI, 2021. *(referência oficial da disciplina)*
- SCHWABER, Ken; SUTHERLAND, Jeff. **O Guia do Scrum**. Scrum.org, 2020. Disponível em: [scrumguides.org](https://scrumguides.org/docs/scrumguide/v2020/2020-Scrum-Guide-PortugueseBR.pdf) *(versão oficial em português)*
- ANDERSON, David J. **Kanban: Successful Evolutionary Change for Your Technology Business**. Blue Hole Press, 2010.
- CROLL, Alistair; YOSKOVITZ, Benjamin. **Lean Analytics**. O'Reilly, 2013. *(gestão orientada a dados e métricas em projetos de produto)*
- HUMBLE, Jez; FARLEY, David. **Continuous Delivery**. Addison-Wesley, 2010. *(ciclo de vida de projetos de software e dados em ambientes ágeis)*

### Documentação oficial

- [PMI — Project Management Institute](https://www.pmi.org/learning/library) — Biblioteca de recursos e padrões do PMI
- [Scrum.org](https://www.scrum.org/resources/scrum-guide) — Guia oficial do Scrum e recursos de certificação
- [Agile Manifesto](https://agilemanifesto.org/iso/ptbr/manifesto.html) — Manifesto Ágil em português
- [GitHub REST API](https://docs.github.com/en/rest) — Extração de dados de projetos e issues via API
- [Plotly](https://plotly.com/python/) — Visualização de cronogramas, burndowns e métricas de projeto
- [Trello](https://trello.com/guide) — Ferramenta visual de gestão de projetos no estilo Kanban

---

## Estrutura de pastas

```
08-metodologias-gestao-projetos/
├── notebooks/
│   ├── 01_estrutura_wbs.ipynb
│   ├── 02_cronograma_gantt.ipynb
│   ├── 03_gestao_de_riscos.ipynb
│   ├── 04_metricas_ageis.ipynb
│   ├── 05_kanban_simulacao.ipynb
│   └── 06_encerramento_licoes.ipynb
├── dados/
│   ├── raw/
│   └── processed/
├── referencias/
│   └── artigos/
└── README.md
```

---

> [← Voltar ao repositório principal](../../README.md)