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

Os arquivos desta unidade contêm exemplos curtos organizados em blocos e **não possuem saídas salvas**. A ausência de saída não equivale a resposta em branco.

| Notebook | Conteúdo observado |
| --- | --- |
| [Árvore de regressão](notebooks/unidade-04-regressao/arvore-de-regressao.ipynb) | Exemplo de árvore e floresta para regressão, com cálculo de MSE e R². |
| [Método dos gradientes descendentes](notebooks/unidade-04-regressao/metodo-dos-gradientes-descendentes.ipynb) | Uso de SGDRegressor em dados pequenos construídos no código. |
| [Método dos mínimos quadrados](notebooks/unidade-04-regressao/metodos-dos-minimos-quadrados.ipynb) | Regressão linear com LinearRegression, previsões, MSE e R². |
| [Regressão regularizada: Lasso, Ridge e ElasticNet](notebooks/unidade-04-regressao/regressao-lasso-ridge-elasticnet.ipynb) | Exemplos dos três regressores regularizados em dados pequenos construídos no código. |
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

MovieLens usa `scikit-surprise==1.1.5`, sem downgrade forçado de NumPy ou encerramento automático da sessão. A preparação registra as versões e solicita reinicialização manual se uma versão antiga já estiver carregada. Online Retail prepara o adaptador Pandas de KaggleHub e `openpyxl`. Seus dois usos de K-Means declaram `n_init=10`; o modelo final também fixa `random_state=42`.

As cargas de Online Retail e MovieLens fixam a versão 1 dos respectivos handles KaggleHub. Online Retail seleciona explicitamente a aba `Year 2009-2010` de `online_retail_II.xlsx`: 525.461 registros de 01/12/2009 a 09/12/2010, antes da limpeza, conforme conferência integral de 2026-10-19. A segunda aba, `Year 2010-2011`, não integra essa prática. O esquema e a conversão de datas são validados antes do processamento; a contagem e o período efetivos continuam sendo exibidos pelo notebook.

MovieLens valida o esquema de `ratings.csv`, preserva os IDs brutos inteiros e utiliza notas na faixa de 0,5 a 5 nos dois Reader. O modelo final recebe o dicionário completo de parâmetros selecionado por RMSE. A consulta do usuário 610 ao item 10 exige que ambos existam individualmente no treino, sem exigir uma avaliação anterior desse par. As saídas antigas não representam novas previsões ou métricas após essas correções.

O exemplo Atari prepara Gymnasium 1.4.0 e ALE 0.12.1, registra `BreakoutNoFrameskip-v4`, empilha quadros com `FrameStackObservation` e diferencia término natural de truncamento. A instalação das dependências requer acesso à rede na sessão.

## Estado de preservação

A documentação foi conferida por leitura dos arquivos em 2026-10-15, sem executar notebooks. A manutenção dos insumos reorganizou o CSV e ajustou a preparação e a leitura de dados da prática de Pandas. Respostas pendentes e saídas históricas foram preservadas. A manutenção de compatibilidade atualizou os critérios dos regressores, as preparações de KaggleHub e MovieLens e a API do Gymnasium no Atari. Os casos alterados foram verificados com ensaios isolados; a execução integral dos notebooks em Colab permanece pendente.

Parte dos materiais depende de downloads de datasets, bibliotecas e serviços externos. As saídas persistidas registram o estado histórico dos arquivos.

## Revisão das saídas em 20/10/2026

Python, Pandas, Perceptron, Online Retail e MovieLens identificam no início as divergências entre fontes corrigidas e saídas históricas. A prática de Pandas usa a coluna `Platform` do CSV original e mantém o comentário fora do comando `%matplotlib inline`; uma cópia completa foi validada localmente: 25 células de código não vazias executadas, cinco células vazias preservadas e três gráficos. Os resultados originais não foram substituídos por essa cópia.

A execução integral no Colab está pendente. Os cinco exemplos de regressão, Fashion MNIST e Atari continuam sem saídas registradas, sem preenchimento de atividades ou criação de resultados. Consulte o [estado de execução](../../docs/estado-execucao.md).

[Voltar ao repositório principal](../../README.md)
