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
| [Pré-processamento com stemming](notebooks/unidade-02/pre-processamento-com-stemming.ipynb) | Pré-processamento de resenhas com SnowballStemmer, representação Bag-of-Words e codificação dos rótulos, preparando os dados para classificação. O notebook termina nessa preparação, sem ajustar um classificador. |
| [Classificação com Bag-of-Words e stemming — variante](notebooks/unidade-02/classificacao-bag-of-words-com-stemming-alternativo.ipynb) | Variante de classificação de resenhas com Bag-of-Words. A preparação final redefine a função anterior e aplica SnowballStemmer. |
| [Representação TF-IDF](notebooks/unidade-02/representacao-tf-idf.ipynb) | Vetorização com TfidfVectorizer e classificação de sentimentos. |
| [Classificação com TF-IDF](notebooks/unidade-02/classificacao-com-tf-idf.ipynb) | Preparação de resenhas, representação TF-IDF e avaliação de classificador. |
| [Classificação com DNN](notebooks/unidade-02/classificacao-com-dnn.ipynb) | Classificação de sentimentos com representação textual vetorizada e rede densa. |
| [Classificação com DNN — alternativo](notebooks/unidade-02/classificacao-com-dnn-alternativo.ipynb) | Versão alternativa do exercício com representação TF-IDF e rede densa. |

## Unidade 03 — Embeddings e redes convolucionais

| Notebook | Conteúdo observado |
| --- | --- |
| [Classificação com word embedding](notebooks/unidade-03/classificacao-com-word-embedding.ipynb) | Conversão de resenhas em sequências, padding e classificação com camada de embedding. |
| [Classificação com GloVe](notebooks/unidade-03/classificacao-com-glove.ipynb) | Preparação de texto e exploração de vetores pré-treinados GloVe em classificação. |
| [Classificação com CNN](notebooks/unidade-03/classificacao-com-cnn.ipynb) | Classificação de resenhas com CNN e embedding treinável de 128 dimensões; a exploração GloVe é opcional e não inicializa a rede. |
| [Classificação com CNN — alternativo](notebooks/unidade-03/classificacao-com-cnn-alternativo.ipynb) | Três modelos com sequências de texto: embedding treinável com pooling global, embedding inicializado por GloVe com pooling global e CNN. |

## Unidade 04 — Redes recorrentes e combinações

| Notebook | Conteúdo observado |
| --- | --- |
| [Classificação com LSTM](notebooks/unidade-04/classificacao-com-lstm.ipynb) | Classificador recorrente que utiliza matriz GloVe na camada de embedding, com pesos congelados. |
| [Classificação com LSTM — alternativo](notebooks/unidade-04/classificacao-com-lstm-alternativo.ipynb) | Dois modelos, LSTM e CNN/LSTM com dropout, com embeddings treináveis de 128 dimensões. A exploração GloVe é opcional e as alternativas comentadas não participam da execução. |
| [Classificação com LSTM e embedding treinável](notebooks/unidade-04/classificacao-com-lstm-embedding-treinavel.ipynb) | Classificador LSTM com embedding treinável de 128 dimensões. A matriz GloVe é preparada em exploração opcional, sem inicializar o modelo. |
| [Classificação com CNN/LSTM](notebooks/unidade-04/classificacao-com-cnn-lstm.ipynb) | Combinação CNN/LSTM com embedding treinável de 128 dimensões. A exploração GloVe é opcional; a alternativa comentada com pesos pré-treinados não está ativa. |
| [Classificação com CNN/LSTM e dropout](notebooks/unidade-04/classificacao-com-cnn-lstm-dropout.ipynb) | Variação CNN/LSTM com dropout e embedding treinável de 128 dimensões. A exploração GloVe é opcional e não inicializa o modelo. |

## Unidade 05 — Entidades nomeadas e tradução

| Notebook | Conteúdo observado |
| --- | --- |
| [Reconhecimento de entidades nomeadas](notebooks/unidade-05/reconhecimento-de-entidades-nomeadas.ipynb) | Aplicação do modelo de português do spaCy a uma frase, com identificação de entidades. |
| [Tradução com Seq2Seq](notebooks/unidade-05/traducao-com-seq2seq.ipynb) | Preparação de pares inglês/português, codificação de caracteres, encoder/decoder LSTM, treinamento e geração de traduções. |
| [Tradução com Seq2Seq — alternativo](notebooks/unidade-05/traducao-com-seq2seq-alternativo.ipynb) | Versão alternativa do exemplo de tradução com encoder/decoder e geração caractere a caractere. |

## Dados e recursos identificados

- As 16 práticas com resenhas IMDb carregam `IMDB Dataset.csv` pelo KaggleHub, com o handle `lakshmi25npathi/imdb-dataset-of-50k-movie-reviews/versions/1`. As cinco cargas anteriormente feitas pelo Drive foram unificadas após comparação integral em 2026-10-19: mesmo SHA-256 e mesma ordem das 50.000 linhas. Não houve deduplicação ou mudança de população. Cada carga valida as colunas `review` e `sentiment`, resenhas textuais não vazias e rótulos `positive`/`negative`. Esses dados não são apresentados como coleta própria.
- Os exercícios introdutórios utilizam recursos de corpus do NLTK; o exemplo de entidades usa um modelo pré-treinado do spaCy.
- A [pasta GloVe](dados/glove/README.md) documenta o recurso pré-treinado de Stanford e sua obtenção. O arquivo de vetores não é versionado neste repositório.
- Os pares de tradução estão em [por.txt](dados/traducao/por.txt), também distribuídos no [arquivo compactado](dados/traducao/por-eng.zip). O [_about.txt](dados/traducao/_about.txt) informa a origem em ManyThings/Tatoeba, a data do conjunto e os termos de uso/atribuição; as linhas do corpus conservam atribuições individuais.

Os arquivos de entrada mantidos manualmente estão em [dados/](dados/README.md), ao lado de notebooks/. Oito notebooks referenciam GloVe: três aplicam a matriz em pelo menos um modelo e cinco mantêm uma exploração opcional sem integração ao classificador. Esses oito notebooks e os dois Seq2Seq possuem uma preparação inicial que localiza o repositório e define os caminhos dos insumos. No Colab, essa preparação clona o repositório somente quando ainda não existe na sessão. Nos cinco blocos exploratórios, `EXPLORAR_GLOVE = False` permite executar o classificador sem o arquivo. Para ativá-los, obtenha e envie manualmente o arquivo conforme [as instruções](dados/glove/README.md), altere o controle para `True` e execute novamente a preparação e as células exploratórias. Os três exemplos que integram a matriz continuam exigindo o arquivo; o corpus de tradução acompanha o Git. Mudanças locais só chegam ao clone do Colab após publicação no remoto.

A autoria individual de cada trecho de notebook e a extensão das adaptações não estão discriminadas nesta coleção. Os exemplos e suas variações são preservados como material acadêmico.

## Estado de preservação e leitura dos resultados

Conferência documental em 2026-10-19. Todos conservam alguma saída histórica. Os caminhos dos insumos GloVe e do corpus de tradução foram organizados em dados/, com preparação inicial da sessão. A manutenção de compatibilidade foi verificada por ensaios isolados com células selecionadas, dimensões e entradas artificiais; a reprodução integral dos notebooks no Colab permanece pendente.

Foram atualizados os imports de Keras e das matrizes de confusão, as declarações de entrada dos modelos com Embedding, o otimizador do segundo modelo CNN alternativo e a agenda de aprendizado do Seq2Seq alternativo. Os exercícios iniciais usam NLTK 3.10.3; os exemplos que baixavam apenas `punkt` passaram a preparar `punkt_tab`. A tokenização legada de Keras foi mantida para preservar os exercícios e seu mapeamento de vocabulário.

As preparações do KaggleHub instalam o extra `pandas-datasets`. Os diagramas Seq2Seq verificam pydot e Graphviz; a instalação de Graphviz, se necessária, ocorre no Colab, enquanto o ambiente local precisa do programa `dot` no PATH. O exemplo de entidades prepara o modelo português do spaCy e informa as versões do pacote e do modelo. Permanecem downloads de dados e modelos externos.

As métricas de classificação correspondem a experimentos educacionais salvos. Nos exemplos Seq2Seq, a demonstração final reutiliza exemplos incluídos na preparação do treinamento e apresenta traduções de qualidade variável; ela não constitui avaliação independente da qualidade de tradução.

Os nomes e as explicações foram alinhados ao código observado, preservando algoritmos e resultados salvos. As alterações de compatibilidade mantêm dimensões, pesos de entrada e opções dos modelos; no Seq2Seq alternativo, o argumento antigo de decaimento foi representado por uma agenda explícita. A exploração GloVe foi explicitada como opcional nos cinco exemplos em que a matriz não alimenta o classificador.

## Revisão das saídas em 20/10/2026

Os 18 notebooks com divergências documentadas identificam no início os registros históricos afetados: versões de bibliotecas, nomes de classes, rótulos de validação, exploração opcional de GloVe, montagem/caminhos antigos do Drive e diagnóstico spaCy. As saídas e os contadores foram preservados. A indicação de histórico evita interpretar esses números e logs como execução da fonte atual.

Na revisão técnica de 20/10/2026, os dois vetorizadores pendentes passaram a usar `min_df=1` e `max_df=1.0`, e a demonstração CNN alternativa passou a selecionar a resenha por posição. Nos dois Seq2Seq, `sample_weight` e `weighted_metrics` excluem posições sem caractere-alvo da acurácia de treino e validação. A perda conserva sua normalização original; as acurácias históricas incluem padding e não foram recalculadas. A integração foi verificada em modelos locais mínimos com dados artificiais e pesos fixos, sem reproduzir o treinamento do corpus ou a sessão Colab.

A execução integral no Colab e a renovação das saídas estão pendentes. O pré-processamento com stemming conserva seu término na preparação/codificação dos dados. Consulte o [estado de execução](../../docs/estado-execucao.md).

[Voltar ao repositório principal](../../README.md)
