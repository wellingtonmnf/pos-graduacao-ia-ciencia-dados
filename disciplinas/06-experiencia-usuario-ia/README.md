# 06 · Experiência de Usuário e IA

> Disciplina do curso de Pós-Graduação em Inteligência Artificial e Ciência de Dados — UNIFACS.

---

## Sobre a disciplina

A disciplina de Experiência de Usuário e IA investiga a interseção entre o design centrado no ser humano e o desenvolvimento de sistemas inteligentes. Projetar uma solução de IA tecnicamente sofisticada não é suficiente se ela não for compreensível, confiável e utilizável pelas pessoas a quem se destina. Esta disciplina forma a competência de pensar o usuário antes do algoritmo — definindo quando e como a máquina deve agir, onde o humano deve permanecer no controle, e como tornar decisões automatizadas transparentes e acessíveis.

---

## Conteúdo programático

### Fundamentos de UX

- Princípios básicos da experiência de usuário
- UX aplicada ao desenvolvimento de iniciativas de inteligência artificial
- Arquiteturas de interação humano-máquina

### Comportamento do consumidor

- Comportamento do consumidor digital
- Modelos mentais e expectativas do usuário frente a sistemas de IA
- Confiança, percepção de risco e aceitação tecnológica

### Metodologia de pesquisa

- Fundamentos em metodologia de pesquisa em UX
- Pesquisa qualitativa e quantitativa com usuários
- Entrevistas, testes de usabilidade e análise de dados comportamentais

### Design centrado no usuário

- Princípios e processo de desenho centrado no usuário (DCU)
- Prototipação e iteração
- Acessibilidade em sistemas de IA

### Divisão de tarefas humano-máquina

- Estratégias para a divisão de tarefas entre humano e máquina
- Automação com supervisão humana
- IA explicável (XAI) e transparência algorítmica
- Ética e viés em sistemas de IA

---

## Notebooks e materiais

| Material | Tópico | Descrição |
|----------|--------|-----------|
| `01_pesquisa_com_usuarios.ipynb` | Metodologia | Análise quantitativa de dados de pesquisa com usuários: surveys e métricas de usabilidade |
| `02_analise_comportamental.ipynb` | Comportamento | Análise de dados de comportamento: cliques, fluxos de navegação e funis de conversão |
| `03_modelos_de_confianca.ipynb` | Confiança | Modelagem estatística de fatores que influenciam a confiança do usuário em sistemas de IA |
| `04_xai_explicabilidade.ipynb` | XAI | Técnicas de IA explicável: SHAP, LIME e visualização de decisões de modelos |
| `05_vies_algoritmico.ipynb` | Ética | Detecção e mitigação de viés em modelos de machine learning |
| `06_prototipo_ia_centrada.ipynb` | Design | Documentação e análise de um protótipo de interface para sistema de IA |

> Esta disciplina combina análise de dados com reflexão crítica sobre design e ética. Os notebooks focam na dimensão quantitativa; os documentos na pasta `referencias/` cobrem os fundamentos conceituais.

---

## Datasets utilizados

| Dataset | Origem | Utilizado em |
|---------|--------|--------------|
| Adult Income (UCI) | [UCI ML Repository](https://archive.ics.uci.edu/dataset/2/adult) | Detecção de viés algorítmico |
| E-commerce Clickstream | [Kaggle](https://www.kaggle.com/datasets/tunguz/online-retail) | Análise de comportamento do consumidor |
| COMPAS Recidivism | [ProPublica](https://github.com/propublica/compas-analysis) | Ética e viés em sistemas de IA |
| SUS Survey Data | Gerado | Análise de métricas de usabilidade (System Usability Scale) |

> Datasets externos são versionados com [Git LFS](https://git-lfs.com/) e estão na pasta `dados/`.

---

## Referências

### Livros e artigos

- NORMAN, Don. **O Design do Dia a Dia**. Rocco, 2006. *(fundamento clássico de design centrado no usuário)*
- RUSSELL, Stuart; NORVIG, Peter. **Artificial Intelligence: A Modern Approach**. 4. ed. Pearson, 2020. *(capítulos sobre IA e interação humano-máquina)*
- AMERSHI, Saleema et al. **Guidelines for Human-AI Interaction**. ACM CHI, 2019. Disponível em: [dl.acm.org/doi/10.1145/3290605.3300233](https://dl.acm.org/doi/10.1145/3290605.3300233)
- LUNDBERG, Scott; LEE, Su-In. **A Unified Approach to Interpreting Model Predictions (SHAP)**. NeurIPS, 2017. Disponível em: [arxiv.org/abs/1705.07874](https://arxiv.org/abs/1705.07874)
- RIBEIRO, Marco Tulio et al. **"Why Should I Trust You?": Explaining the Predictions of Any Classifier (LIME)**. KDD, 2016. Disponível em: [arxiv.org/abs/1602.04938](https://arxiv.org/abs/1602.04938)

### Documentação oficial

- [SHAP](https://shap.readthedocs.io/en/latest/) — Explicabilidade de modelos de machine learning
- [LIME](https://lime-ml.readthedocs.io/en/latest/) — Explicações locais para qualquer classificador
- [Fairlearn](https://fairlearn.org/v0.10/user_guide/index.html) — Avaliação e mitigação de viés em modelos
- [Google PAIR Guidebook](https://pair.withgoogle.com/guidebook/) — Guia prático de design de produtos com IA
- [Microsoft HAX Toolkit](https://www.microsoft.com/en-us/haxtoolkit/) — Toolkit de interação humano-IA da Microsoft
- [Nielsen Norman Group — AI UX](https://www.nngroup.com/topic/artificial-intelligence/) — Artigos e pesquisas sobre UX em sistemas de IA

---

## Estrutura de pastas

```
06-experiencia-usuario-ia/
├── notebooks/
│   ├── 01_pesquisa_com_usuarios.ipynb
│   ├── 02_analise_comportamental.ipynb
│   ├── 03_modelos_de_confianca.ipynb
│   ├── 04_xai_explicabilidade.ipynb
│   ├── 05_vies_algoritmico.ipynb
│   └── 06_prototipo_ia_centrada.ipynb
├── dados/
│   ├── raw/
│   └── processed/
├── referencias/
│   └── artigos/
└── README.md
```

---

> [← Voltar ao repositório principal](../../README.md)