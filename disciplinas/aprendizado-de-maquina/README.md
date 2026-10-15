# Aprendizado de Máquina

Registro de notebooks e exercícios preservados da pós-graduação em Inteligência Artificial e Ciência de Dados. Este catálogo descreve os **18 arquivos existentes**, incluindo exemplos adaptados de terceiros e materiais com respostas parciais.

## Unidade 01 — Python e manipulação de dados

| Notebook | Conteúdo observado |
| --- | --- |
| [Prática 1 — Aprendendo Python](notebooks/unidade-01-introducao/pratica-1-aprendendo-python.ipynb) | Enunciados de exercícios sobre entrada de dados, condicionais, laços, listas, funções e strings. O cálculo salarial tem implementação e saída salva; as demais respostas contêm principalmente exemplos comentados. |
| [Prática 2 — Aprendendo Pandas](notebooks/unidade-01-introducao/pratica-2-aprendendo-pandas.ipynb) | Material sobre NumPy, Pandas e Matplotlib, com dados de vendas de videogames. Há exemplos comentados, saídas históricas e respostas de atividades em branco. |

O [CSV de vendas de videogames](dados/at2-vgsales.csv) acompanha a segunda prática. O notebook identifica sua origem como Video Game Sales, disponibilizado no Kaggle por Gregor Utrecht.

## Unidade 02 — Classificação

| Notebook | Conteúdo observado |
| --- | --- |
| [Árvore de decisão](notebooks/unidade-02-classificacao/algoritmo-arvore-de-decisao.ipynb) | Classificação de Iris, separação treino/teste, métricas, matriz de confusão e visualização da árvore. |
| [Curva ROC e AUC](notebooks/unidade-02-classificacao/algoritmo-curva-roc-e-auc.ipynb) | Dados sintéticos, regressão logística, probabilidades, ROC/AUC e exploração de limiares. |
| [K-Nearest Neighbors](notebooks/unidade-02-classificacao/algoritmo-k-nearest-neighbors.ipynb) | KNN sobre Iris, com treino/teste e relatório de classificação. |
| [Naive Bayes gaussiano](notebooks/unidade-02-classificacao/algoritmo-naive-bayes-gaussiano.ipynb) | GaussianNB sobre Iris, avaliação e matriz de confusão. |
| [Regressão logística](notebooks/unidade-02-classificacao/algoritmo-regressao-logistica.ipynb) | Classificação de Iris com regressão logística e avaliação sobre conjunto de teste. |
| [SVM linear](notebooks/unidade-02-classificacao/algoritmo-svm-linear.ipynb) | Classificação de Iris com SVC de kernel linear e métricas. |
| [Redes neurais artificiais](notebooks/unidade-02-classificacao/redes-neurais-artificiais.ipynb) | Perceptron em exemplo de três alunos; previsões e avaliação sobre os próprios dados de treinamento. |

Esses notebooks conservam saídas. As métricas descrevem os exemplos salvos e seus respectivos recortes de avaliação; a avaliação do Perceptron não utiliza dados separados para teste.

## Unidade 03 — Clusterização e recomendação

| Notebook | Conteúdo observado |
| --- | --- |
| [Clusterização — Online Retail](notebooks/unidade-03-clusterizacao/pratica-de-clusterizacao-online-retail.ipynb) | Carregamento via KaggleHub, limpeza, atributos RFM, padronização, K-Means, silhouette e agrupamento hierárquico, com saídas salvas. |
| [Recomendação — MovieLens](notebooks/unidade-03-clusterizacao/sistema-de-recomendacao-movielens.ipynb) | Filtragem colaborativa com scikit-surprise, filtragem de avaliações, comparação de algoritmos e busca de parâmetros, com saídas salvas. |

## Unidade 04 — Regressão

Cada arquivo desta unidade contém uma célula de código e **não possui saídas salvas**. São exemplos curtos preservados; ausência de saída não equivale a resposta em branco.

| Notebook | Conteúdo observado |
| --- | --- |
| [Árvore de regressão](notebooks/unidade-04-regressao/arvore-de-regressao.ipynb) | Exemplo de árvore e floresta para regressão, com cálculo de MSE e R². |
| [Método dos gradientes descendentes](notebooks/unidade-04-regressao/metodo-dos-gradientes-descendentes.ipynb) | Uso de SGDRegressor em dados pequenos construídos no código. |
| [Método dos mínimos quadrados](notebooks/unidade-04-regressao/metodos-dos-minimos-quadrados.ipynb) | Regressão linear com LinearRegression, previsões, MSE e R². |
| [SGD Regressor — nome preservado](notebooks/unidade-04-regressao/sgd-regressor.ipynb) | Apesar do nome, o código contém exemplos de Lasso, Ridge e ElasticNet. |
| [SVR](notebooks/unidade-04-regressao/svr.ipynb) | Regressão com máquinas de vetores de suporte e métricas sobre os dados usados no ajuste. |

## Unidade 05 — Redes neurais e Deep Learning

| Notebook | Conteúdo observado |
| --- | --- |
| [Classificação básica de imagens de roupas](notebooks/unidade-05-redes-neurais-e-deep-learning/classificacao-basica-imagens-de-roupas.ipynb) | Tutorial de classificação de Fashion MNIST com TensorFlow/Keras, preparação de imagens, treinamento, avaliação e previsões. Sem saídas salvas. |
| [Deep Q-Learning — Atari Breakout](notebooks/unidade-05-redes-neurais-e-deep-learning/deep-q-learning-atari-breakout.ipynb) | Exemplo de Deep Q-Network para Atari Breakout com Keras e Gymnasium. Sem saídas de execução salvas; as animações são referências externas do material. |

## Origens identificadas nos materiais

- **Python/Pandas e Matplotlib:** a segunda prática declara adaptação de tutoriais de Paulo Vasconcellos; os links originais permanecem no notebook.
- **Online Retail:** o notebook declara Wellington Morais como autor do experimento e informa que se baseia no exemplo de Manish Kumar, no Kaggle. Essa atribuição de adaptação é preservada.
- **MovieLens:** o notebook declara base no exemplo de Kuldeep Singh, no repositório `singhsidhukuldeep/Recommendation-System`.
- **Fashion MNIST:** material com atribuição a The TensorFlow Authors e links para o tutorial oficial do TensorFlow.
- **Atari Breakout:** material com autoria atribuída a Jacob Chapman e Mathias Lechner.

As atribuições acima seguem as declarações dos próprios notebooks. Os demais arquivos não discriminam a origem de cada trecho ou a extensão das adaptações.

## Insumos e preparação da sessão

Os arquivos de entrada mantidos no repositório ficam em [dados/](dados/README.md), ao lado de notebooks/. A prática de Pandas define REPO_DIR, DISCIPLINA_DIR, DATA_DIR e CSV_PATH na preparação inicial e utiliza o CSV dessa pasta. No Colab, a célula obtém uma cópia do repositório caso ainda não exista em /content; em uma cópia local, procura a raiz a partir do diretório da sessão. Alterações locais precisam ser publicadas antes de ficarem disponíveis pelo clone no Colab; cópias antigas na sessão precisam ser atualizadas.

As bases obtidas pelo próprio código, como Online Retail via KaggleHub, MovieLens e Fashion MNIST, continuam com seus mecanismos de obtenção. Esta organização não replica seus caches.

## Estado de preservação

A documentação foi conferida por leitura dos arquivos em 2026-10-15, sem executar notebooks. A manutenção dos insumos reorganizou o CSV e ajustou a preparação e a leitura de dados da prática de Pandas. Respostas pendentes e saídas históricas foram preservadas. O ambiente de execução ainda não foi validado.

Parte dos materiais depende de downloads de datasets, bibliotecas e serviços externos. As saídas persistidas registram o estado histórico dos arquivos.

[Voltar ao repositório principal](../../README.md)
