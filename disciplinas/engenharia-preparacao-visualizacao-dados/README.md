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

Conferência documental em 2026-10-15, por leitura, sem execução. As imagens foram organizadas e os caminhos de entrada e saída ajustados, com preparação inicial da sessão. Os usos de K-Means que dependiam do valor padrão de `n_init` agora declaram `n_init=10`. Esses exemplos pequenos foram executados em ensaios isolados; as saídas históricas permanecem preservadas.

Os resultados salvos fazem parte do registro acadêmico; a reprodução integral no Colab ainda não foi validada.

## Revisão das saídas em 20/10/2026

Os exemplos K-Means simples e K-Means random-state identificam no início as saídas históricas que já não correspondem aos prints ou às comparações atuais. Os resultados foram preservados. A execução integral no Colab e a geração de novas figuras e métricas permanecem pendentes; consulte o [estado de execução](../../docs/estado-execucao.md).

## Tamanho das figuras — 20/10/2026

O notebook de processamento de imagens define tamanhos locais: 10 × 10 polegadas a 100 DPI nas duas visualizações de imagem e 8 × 4 polegadas a 100 DPI no histograma. A configuração global de 224 × 224 polegadas foi removida. Os arquivos de entrada mantêm suas dimensões originais; as figuras salvas no notebook são históricas e não foram recalculadas.

[Voltar ao repositório principal](../../README.md)
