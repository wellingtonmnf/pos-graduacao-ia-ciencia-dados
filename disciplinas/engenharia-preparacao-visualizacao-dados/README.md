# Engenharia, Preparação e Visualização de Dados

Registro de **cinco notebooks** preservados da pós-graduação em Inteligência Artificial e Ciência de Dados. O catálogo corresponde aos exercícios disponíveis: representação de texto, agrupamento e processamento de imagens. Os arquivos estão reunidos na pasta `notebooks/`, sem subdivisão por unidade.

## Notebooks

| Notebook | Conteúdo observado |
| --- | --- |
| [Bag-of-words](notebooks/bag-of-words.ipynb) | CountVectorizer em quatro frases: vocabulário e matriz de contagem de termos, com saídas salvas. |
| [K-Means](notebooks/k-means.ipynb) | Agrupamento de seis pontos, rótulos, centroides e previsão de grupos para novos pontos. Conserva saídas. |
| [K-Means — aprofundamento](notebooks/k-means-aprofundado.ipynb) | Exploração de inicialização, sementes pseudoaleatórias, centroides, inércia e distâncias, com saídas salvas. |
| [K-Means — random_state](notebooks/k-means-random-state.ipynb) | Dados sintéticos e comparação de execuções com e sem semente fixa, incluindo centroides e inércia. Conserva saídas. |
| [Processamento de imagem](notebooks/processamento-de-imagem.ipynb) | Leitura e visualização com OpenCV/Matplotlib, detecção de faces com Haar Cascade, máscara e histogramas de cores. Conserva saídas. |

Os três arquivos de K-Means exploram variações relacionadas do mesmo conceito.

## Materiais e origem

Os exemplos de agrupamento e texto constroem seus dados no próprio código. O notebook de imagens referencia arquivos locais de entrada e saída e identifica o exemplo de histogramas como proveniente da documentação do OpenCV. A autoria de cada trecho e o grau de adaptação dos demais exemplos não estão discriminados nos arquivos.

## Insumos e preparação da sessão

As quatro imagens fornecidas estão em [dados/imagens/](dados/imagens/), com descrição em [dados/README.md](dados/README.md): imagem.png, alguns.jpg, muitos.jpg e histograma.png. A entrada ativa do notebook é muitos.jpg; imagem.png e alguns.jpg são alternativas comentadas. histograma.png acompanha o acervo e não é lido pelo código atual.

Execute a preparação inicial do notebook de processamento de imagem antes das demais células. Ela define os caminhos da disciplina, utiliza uma cópia local do repositório ou obtém uma no Colab quando ainda não existir em /content. Alterações locais precisam ser publicadas para ficarem disponíveis pelo clone no Colab; cópias antigas na sessão precisam ser atualizadas. Não é necessário montar um Drive pessoal.

A pasta resultados/ é criada na execução e ignorada pelo Git. todos.jpg é gerado pelo exercício e relido nas células seguintes; aragorn.png e poucos.jpg permanecem apenas como alternativas comentadas de saída. Nenhum desses resultados é tratado como imagem de entrada fornecida.

## Estado de preservação

Conferência documental em 2026-10-15, por leitura, sem execução. As imagens foram organizadas e os caminhos de entrada e saída ajustados, com preparação inicial da sessão. As demais células e saídas históricas foram preservadas; a compatibilidade do ambiente ainda precisa ser conferida antes da reprodução.

Os resultados salvos fazem parte do registro acadêmico; a execução atual ainda não foi validada.

[Voltar ao repositório principal](../../README.md)
