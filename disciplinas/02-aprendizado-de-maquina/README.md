# 02 · Aprendizado de Máquina

> Disciplina do curso de Pós-Graduação em Inteligência Artificial e Ciência de Dados — UNIFACS.

---

## Sobre a disciplina

Aprendizado de Máquina (Machine Learning) é o campo da Inteligência Artificial dedicado ao desenvolvimento de sistemas capazes de aprender a partir de dados, identificar padrões e tomar decisões com o mínimo de intervenção humana. Esta disciplina cobre desde os fundamentos teóricos até as principais técnicas e frameworks utilizados na prática.

---

## Conteúdo programático

### Fundamentos

- Introdução ao Aprendizado de Máquina
- Sistemas Especialistas
- Visão geral das abordagens de aprendizado

### Aprendizado Supervisionado

- Algoritmos de Aprendizado Supervisionado
- Classificação
- Regressão
- Sistemas de recomendação

### Aprendizado Não Supervisionado

- Algoritmos de Aprendizado Não Supervisionado
- Técnicas de agrupamento (clustering)

### Redes Neurais e Deep Learning

- Fundamentos de Redes Neurais Artificiais
- Deep Learning
- Arquiteturas e aplicações

### Aprendizado por Reforço

- Aprendizado por Reforço (Reinforcement Learning)
- Processo de Decisão de Markov (MDP)

### Linguagem Natural e Dados Textuais

- Processamento de Texto
- Análise de Sentimentos

### Aplicações e Ferramentas

- Principais aplicações de Aprendizado de Máquina
- Linguagens de programação e frameworks: Python, Scikit-learn, TensorFlow, PyTorch

---

## Notebooks

| Notebook | Tópico | Descrição |
|----------|--------|-----------|
| `01_introducao_ml.ipynb` | Fundamentos | Conceitos básicos, tipos de aprendizado e fluxo geral de um projeto de ML |
| `02_regressao_linear.ipynb` | Supervisionado | Regressão linear simples e múltipla com Scikit-learn |
| `03_classificacao.ipynb` | Supervisionado | Árvores de decisão, KNN e SVM |
| `04_clustering_kmeans.ipynb` | Não Supervisionado | Agrupamento com K-Means e análise de clusters |
| `05_redes_neurais.ipynb` | Deep Learning | Construção de uma rede neural simples com TensorFlow/Keras |
| `06_analise_sentimentos.ipynb` | Texto | Classificação de texto e análise de sentimentos |

> Os notebooks estão organizados em ordem crescente de complexidade. Recomenda-se seguir essa sequência no primeiro contato com a disciplina.

---

## Datasets utilizados

| Dataset | Origem | Utilizado em |
|---------|--------|--------------|
| Iris | `sklearn.datasets` | Classificação |
| Boston Housing | `sklearn.datasets` | Regressão linear |
| MNIST | `tensorflow.keras.datasets` | Redes neurais |
| IMDb Reviews | Kaggle / HuggingFace | Análise de sentimentos |

> Datasets externos são versionados com [Git LFS](https://git-lfs.com/) e estão na pasta `dados/`.

---

## Referências

### Livros e artigos

- GÉRON, Aurélien. **Mãos à obra: aprendizado de máquina com Scikit-Learn, Keras & TensorFlow**. 2. ed. Alta Books, 2021.
- GOODFELLOW, Ian; BENGIO, Yoshua; COURVILLE, Aaron. **Deep Learning**. MIT Press, 2016. Disponível em: [deeplearningbook.org](https://www.deeplearningbook.org/)
- BISHOP, Christopher M. **Pattern Recognition and Machine Learning**. Springer, 2006.
- MITCHELL, Tom M. **Machine Learning**. McGraw-Hill, 1997.
- HASTIE, Trevor; TIBSHIRANI, Robert; FRIEDMAN, Jerome. **The Elements of Statistical Learning**. 2. ed. Springer, 2009. Disponível em: [web.stanford.edu/~hastie/ElemStatLearn](https://web.stanford.edu/~hastie/ElemStatLearn/)

### Documentação oficial

- [Scikit-learn](https://scikit-learn.org/stable/user_guide.html) — User Guide completo com exemplos
- [TensorFlow](https://www.tensorflow.org/learn) — Tutoriais e guias oficiais
- [PyTorch](https://pytorch.org/tutorials/) — Tutoriais oficiais por nível
- [Keras](https://keras.io/guides/) — Guias de uso da API
- [Pandas](https://pandas.pydata.org/docs/user_guide/index.html) — Manipulação de dados
- [NumPy](https://numpy.org/doc/stable/user/index.html) — Computação numérica

---

## Estrutura de pastas

```
02-aprendizado-de-maquina/
├── notebooks/
│   ├── 01_introducao_ml.ipynb
│   ├── 02_regressao_linear.ipynb
│   ├── 03_classificacao.ipynb
│   ├── 04_clustering_kmeans.ipynb
│   ├── 05_redes_neurais.ipynb
│   └── 06_analise_sentimentos.ipynb
├── dados/
│   ├── raw/
│   └── processed/
├── referencias/
│   └── artigos/
└── README.md
```

---

> [← Voltar ao repositório principal](../../README.md)