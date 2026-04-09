# 05 · Processamento de Linguagem Natural

> Disciplina do curso de Pós-Graduação em Inteligência Artificial e Ciência de Dados — UNIFACS.

---

## Sobre a disciplina

Processamento de Linguagem Natural (PLN ou NLP, do inglês *Natural Language Processing*) é o campo da IA dedicado a fazer com que computadores compreendam, interpretem e gerem linguagem humana. Esta disciplina cobre desde os fundamentos linguísticos e estatísticos até arquiteturas de redes neurais modernas, com aplicações em análise de texto, tradução automática e reconhecimento de voz.

---

## Conteúdo programático

### Fundamentos da linguagem

- Teoria da linguagem
- Modelagem estatística com tokenização

### Representação de texto

- Bag of Words (BoW)
- N-gramas
- TF-IDF (Term Frequency–Inverse Document Frequency)
- Word2Vec — representação vetorial de palavras

### Redes neurais aplicadas a texto

- Redes Neurais Convolucionais (CNN) para texto
- Redes Neurais Recorrentes (RNN)
- LSTM (Long Short-Term Memory)

### Modelos de sequência e voz

- Seq2Seq (sequência para sequência)
- Reconhecimento de voz

---

## Notebooks

| Notebook | Tópico | Descrição |
|----------|--------|-----------|
| `01_tokenizacao_e_normalizacao.ipynb` | Fundamentos | Tokenização, remoção de stopwords, stemming e lematização |
| `02_bag_of_words_tfidf.ipynb` | Representação | Construção de vetores BoW e TF-IDF com Scikit-learn |
| `03_ngramas.ipynb` | Representação | Modelagem de n-gramas e análise de frequência |
| `04_word2vec.ipynb` | Representação | Treinamento e visualização de embeddings com Gensim |
| `05_cnn_texto.ipynb` | Redes Neurais | Classificação de texto com redes convolucionais |
| `06_rnn_lstm.ipynb` | Redes Neurais | Modelagem de sequências com RNN e LSTM |
| `07_seq2seq.ipynb` | Sequências | Arquitetura Seq2Seq para tradução e geração de texto |
| `08_reconhecimento_de_voz.ipynb` | Voz | Introdução ao reconhecimento de voz com SpeechRecognition |

> Os notebooks seguem uma progressão natural: do texto bruto à representação vetorial, e desta às arquiteturas neurais.

---

## Datasets utilizados

| Dataset | Origem | Utilizado em |
|---------|--------|--------------|
| IMDb Reviews | [HuggingFace Datasets](https://huggingface.co/datasets/imdb) | Classificação de sentimentos |
| 20 Newsgroups | `sklearn.datasets` | BoW, TF-IDF e classificação de texto |
| Wikipedia PT-BR (amostra) | [NILC-USP](http://www.nilc.icmc.usp.br/embeddings) | Word2Vec |
| Common Voice | [Mozilla](https://commonvoice.mozilla.org/pt) | Reconhecimento de voz |

> Datasets externos são versionados com [Git LFS](https://git-lfs.com/) e estão na pasta `dados/`.

---

## Referências

### Livros e artigos

- JURAFSKY, Dan; MARTIN, James H. **Speech and Language Processing**. 3. ed. (draft). Stanford, 2023. Disponível em: [web.stanford.edu/~jurafsky/slp3](https://web.stanford.edu/~jurafsky/slp3/)
- BIRD, Steven; KLEIN, Ewan; LOPER, Edward. **Natural Language Processing with Python**. O'Reilly, 2009. Disponível em: [nltk.org/book](https://www.nltk.org/book/)
- VASWANI, Ashish et al. **Attention Is All You Need**. NeurIPS, 2017. Disponível em: [arxiv.org/abs/1706.03762](https://arxiv.org/abs/1706.03762)
- MIKOLOV, Tomas et al. **Efficient Estimation of Word Representations in Vector Space**. arXiv, 2013. Disponível em: [arxiv.org/abs/1301.3781](https://arxiv.org/abs/1301.3781)
- HOCHREITER, Sepp; SCHMIDHUBER, Jürgen. **Long Short-Term Memory**. Neural Computation, 1997.

### Documentação oficial

- [NLTK](https://www.nltk.org/) — Natural Language Toolkit, biblioteca clássica de PLN em Python
- [spaCy](https://spacy.io/usage) — Processamento de texto industrial com modelos prontos
- [Gensim](https://radimrehurek.com/gensim/) — Word2Vec, Doc2Vec e modelagem de tópicos
- [HuggingFace Transformers](https://huggingface.co/docs/transformers/index) — Modelos pré-treinados de última geração
- [SpeechRecognition](https://pypi.org/project/SpeechRecognition/) — Reconhecimento de voz em Python
- [Scikit-learn: Text Feature Extraction](https://scikit-learn.org/stable/modules/feature_extraction.html#text-feature-extraction) — TF-IDF e BoW

---

## Estrutura de pastas

```
05-processamento-linguagem-natural/
├── notebooks/
│   ├── 01_tokenizacao_e_normalizacao.ipynb
│   ├── 02_bag_of_words_tfidf.ipynb
│   ├── 03_ngramas.ipynb
│   ├── 04_word2vec.ipynb
│   ├── 05_cnn_texto.ipynb
│   ├── 06_rnn_lstm.ipynb
│   ├── 07_seq2seq.ipynb
│   └── 08_reconhecimento_de_voz.ipynb
├── dados/
│   ├── raw/
│   └── processed/
├── referencias/
│   └── artigos/
└── README.md
```

---

> [← Voltar ao repositório principal](../../README.md)