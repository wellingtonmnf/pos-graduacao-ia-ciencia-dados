# Processamento de Linguagem Natural

Registro de **21 notebooks** preservados da pós-graduação em Inteligência Artificial e Ciência de Dados, distribuídos em cinco unidades. A coleção reúne exercícios e variações sobre representação de texto, classificação, redes neurais, reconhecimento de entidades e tradução.

## Unidade 01 — Introdução e representação de texto

| Notebook | Conteúdo observado |
| --- | --- |
| [Introdução ao PLN](notebooks/unidade-01/introducao-ao-pln.ipynb) | Exploração de corpus do NLTK, tokenização de sentenças e palavras, tratamento de texto e representação por contagens. |
| [Tokenização e bag-of-words](notebooks/unidade-01/tokenizacao-e-bag-of-words.ipynb) | Tokenização, preparação de texto e matriz de contagem com CountVectorizer. |

## Unidade 02 — Pré-processamento, n-gramas e TF-IDF

| Notebook | Conteúdo observado |
| --- | --- |
| [Análise de n-gramas](notebooks/unidade-02/analise-de-n-gramas.ipynb) | Preparação de resenhas e exploração de representações com sequências de palavras para classificação. |
| [Pré-processamento com stemming](notebooks/unidade-02/pre-processamento-com-stemming.ipynb) | Tokenização, remoção de elementos do texto e redução de palavras com SnowballStemmer, em exemplo de classificação de sentimentos. |
| [Pré-processamento sem stemming](notebooks/unidade-02/pre-processamento-sem-stemming.ipynb) | Variante de preparação e classificação de resenhas. Apesar do nome, o código inclui uma rotina com SnowballStemmer; o nome foi preservado. |
| [Representação TF-IDF](notebooks/unidade-02/representacao-tf-idf.ipynb) | Vetorização com TfidfVectorizer e classificação de sentimentos. |
| [Classificação com TF-IDF](notebooks/unidade-02/classificacao-com-tf-idf.ipynb) | Preparação de resenhas, representação TF-IDF e avaliação de classificador. |
| [Classificação com DNN](notebooks/unidade-02/classificacao-com-dnn.ipynb) | Classificação de sentimentos com representação textual vetorizada e rede densa. |
| [Classificação com DNN — alternativo](notebooks/unidade-02/classificacao-com-dnn-alternativo.ipynb) | Versão alternativa do exercício com representação TF-IDF e rede densa. |

## Unidade 03 — Embeddings e redes convolucionais

| Notebook | Conteúdo observado |
| --- | --- |
| [Classificação com word embedding](notebooks/unidade-03/classificacao-com-word-embedding.ipynb) | Conversão de resenhas em sequências, padding e classificação com camada de embedding. |
| [Classificação com GloVe](notebooks/unidade-03/classificacao-com-glove.ipynb) | Preparação de texto e exploração de vetores pré-treinados GloVe em classificação. |
| [Classificação com CNN](notebooks/unidade-03/classificacao-com-cnn.ipynb) | Classificação de resenhas com embedding e rede convolucional unidimensional. |
| [Classificação com CNN — alternativo](notebooks/unidade-03/classificacao-com-cnn-alternativo.ipynb) | Versão alternativa do exercício com sequências de texto e convolução. |

## Unidade 04 — Redes recorrentes e combinações

| Notebook | Conteúdo observado |
| --- | --- |
| [Classificação com LSTM](notebooks/unidade-04/classificacao-com-lstm.ipynb) | Classificador recorrente que utiliza matriz GloVe na camada de embedding, com pesos congelados. |
| [Classificação com LSTM — alternativo](notebooks/unidade-04/classificacao-com-lstm-alternativo.ipynb) | Variações de classificação com LSTM e combinação CNN/LSTM. |
| [Classificação com LSTM e GloVe — nome preservado](notebooks/unidade-04/classificacao-com-lstm-e-glove.ipynb) | Carrega e prepara matriz GloVe, mas a definição do modelo usa embedding sem receber essa matriz. O nome do arquivo não descreve integralmente o uso efetivo dos vetores. |
| [Classificação com CNN/LSTM](notebooks/unidade-04/classificacao-com-cnn-lstm.ipynb) | Classificador que combina camadas convolucionais e recorrentes. |
| [Classificação com CNN/LSTM e dropout](notebooks/unidade-04/classificacao-com-cnn-lstm-dropout.ipynb) | Variação da combinação CNN/LSTM com regularização por dropout. |

## Unidade 05 — Entidades nomeadas e tradução

| Notebook | Conteúdo observado |
| --- | --- |
| [Reconhecimento de entidades nomeadas](notebooks/unidade-05/reconhecimento-de-entidades-nomeadas.ipynb) | Aplicação do modelo de português do spaCy a uma frase, com identificação de entidades. |
| [Tradução com Seq2Seq](notebooks/unidade-05/traducao-com-seq2seq.ipynb) | Preparação de pares inglês/português, codificação de caracteres, encoder/decoder LSTM, treinamento e geração de traduções. |
| [Tradução com Seq2Seq — alternativo](notebooks/unidade-05/traducao-com-seq2seq-alternativo.ipynb) | Versão alternativa do exemplo de tradução com encoder/decoder e geração caractere a caractere. |

## Dados e recursos identificados

- Os exercícios de classificação utilizam resenhas do IMDb, carregadas por KaggleHub ou por links externos preservados nos notebooks. Esses dados não são apresentados como coleta própria.
- Os exercícios introdutórios utilizam recursos de corpus do NLTK; o exemplo de entidades usa um modelo pré-treinado do spaCy.
- A [pasta GloVe](dados/glove/README.md) documenta o recurso pré-treinado de Stanford e sua obtenção. O arquivo de vetores não é versionado neste repositório.
- Os pares de tradução estão em [por.txt](dados/traducao/por.txt), também distribuídos no [arquivo compactado](dados/traducao/por-eng.zip). O [_about.txt](dados/traducao/_about.txt) informa a origem em ManyThings/Tatoeba, a data do conjunto e os termos de uso/atribuição; as linhas do corpus conservam atribuições individuais.

Os arquivos de entrada mantidos manualmente estão em [dados/](dados/README.md), ao lado de notebooks/. Os oito exemplos com GloVe e os dois Seq2Seq possuem uma preparação inicial que localiza o repositório, define os caminhos dos insumos e informa arquivos ausentes. No Colab, essa preparação clona o repositório somente quando ainda não existe na sessão. O GloVe continua exigindo obtenção e envio manuais; o corpus de tradução acompanha o Git. Mudanças locais só chegam ao clone do Colab após publicação no remoto.

A autoria individual de cada trecho de notebook e a extensão das adaptações não estão discriminadas nesta coleção. Os exemplos e suas variações são preservados como material acadêmico.

## Estado de preservação e leitura dos resultados

Conferência documental em 2026-10-15, por leitura dos arquivos, sem executar notebooks. Todos conservam alguma saída; a reprodução atual ainda não foi validada. Os caminhos dos insumos GloVe e do corpus de tradução foram organizados em dados/, com preparação inicial da sessão. Permanecem dependências de downloads e modelos pré-treinados, e a compatibilidade das bibliotecas ainda precisa de revisão técnica para reprodução.

As métricas de classificação correspondem a experimentos educacionais salvos. Nos exemplos Seq2Seq, a demonstração final reutiliza exemplos incluídos na preparação do treinamento e apresenta traduções de qualidade variável; ela não constitui avaliação independente da qualidade de tradução.

Os nomes, algoritmos, parâmetros e resultados salvos foram preservados nesta etapa; as alterações de código se limitam à preparação da sessão e aos caminhos dos insumos. Diferenças entre títulos e implementação permanecem documentadas.

[Voltar ao repositório principal](../../README.md)
