![Topo Unifacs](assets/unifacs.png)

# Pós-Graduação em Inteligência Artificial e Ciência de Dados

Acervo de notebooks e exercícios acadêmicos preservados de três disciplinas da Pós-Graduação em Inteligência Artificial e Ciência de Dados da UNIFACS.

Os materiais incluem exemplos, exercícios e adaptações de tutoriais, organizados por disciplina. Os catálogos abaixo descrevem o conteúdo dos arquivos disponíveis e registram suas particularidades.

## Disciplinas e notebooks

| Disciplina | Notebooks | Conteúdo presente |
| --- | ---: | --- |
| [Aprendizado de Máquina](disciplinas/aprendizado-de-maquina/README.md) | 18 | Python e Pandas; classificação; agrupamento e recomendação; regressão; redes neurais e aprendizado por reforço |
| [Engenharia, Preparação e Visualização de Dados](disciplinas/engenharia-preparacao-visualizacao-dados/README.md) | 5 | Bag-of-Words, exemplos de K-Means e processamento de imagem |
| [Processamento de Linguagem Natural](disciplinas/processamento-linguagem-natural/README.md) | 21 | Tokenização, pré-processamento, n-gramas, TF-IDF, classificação de texto, embeddings, CNN, LSTM, entidades nomeadas e tradução Seq2Seq |
| **Total** | **44** | A contagem inclui versões alternativas e variações de exemplos |

Os notebooks de Aprendizado de Máquina e Processamento de Linguagem Natural mantêm a organização por unidade. Em Engenharia, Preparação e Visualização de Dados, os arquivos ficam na pasta `notebooks/`, sem subdivisão por unidade.

## Como consultar

Abra o catálogo de uma disciplina e siga os links para os notebooks disponíveis. As descrições se baseiam no código e nas explicações presentes nos arquivos.

O conjunto reúne materiais em diferentes condições: há exemplos com resultados salvos, exercícios com respostas pendentes e código sem saídas registradas. A ausência de saídas, isoladamente, não determina se uma atividade foi concluída. Os resultados persistidos são registros do notebook e não comprovam uma execução atual do código.

## Origem dos materiais

Os notebooks pertencem ao contexto de estudo da pós-graduação e incluem exemplos e adaptações de fontes externas. Quando os arquivos identificam autores ou tutoriais de origem, essas atribuições são indicadas nos catálogos das disciplinas e permanecem nos próprios notebooks.

## Dados e preparação da sessão

Os arquivos de entrada fornecidos manualmente ficam em `dados/`, ao lado de `notebooks/`, na respectiva disciplina. Os arquivos originais e suas informações de origem foram preservados.

| Disciplina | Insumos disponíveis |
| --- | --- |
| [Aprendizado de Máquina](disciplinas/aprendizado-de-maquina/dados/README.md) | CSV de vendas de videogames |
| [Engenharia, Preparação e Visualização de Dados](disciplinas/engenharia-preparacao-visualizacao-dados/dados/README.md) | Imagens fornecidas para os exemplos |
| [Processamento de Linguagem Natural](disciplinas/processamento-linguagem-natural/dados/README.md) | Corpus de tradução e orientações para os vetores GloVe |

Os dados obtidos por bibliotecas, como KaggleHub, scikit-learn, TensorFlow, NLTK e spaCy, continuam usando os mecanismos de carregamento e download presentes nos exemplos. Seus caches não fazem parte da pasta de insumos manuais.

### Google Colab

Cada notebook possui um botão **Abrir no Colab** no início, que abre o próprio arquivo publicado no GitHub. Depois de abrir, execute as células na ordem indicada.

Todos os notebooks foram trabalhados no Google Colab. Nos exemplos que leem arquivos de `dados/`, as células iniciais de preparação localizam o repositório e definem a pasta da disciplina e `DATA_DIR`. Quando o repositório ainda não está na sessão Colab, a preparação obtém um clone público em `/content/pos-graduacao-ia-ciencia-dados`.

1. Abra o notebook no Colab e execute as células iniciais de preparação.
2. Os arquivos pequenos versionados acompanham o clone. GloVe é necessário nos três notebooks que aplicam seus pesos a um modelo; nos outros cinco que exploram os vetores, essa etapa é opcional e começa desativada (`EXPLORAR_GLOVE = False`). Consulte a relação dos exemplos e as [orientações de download e localização](disciplinas/processamento-linguagem-natural/dados/glove/README.md).
3. Continue pelas células do exemplo, observando suas instalações e instruções próprias. A preparação dos arquivos localiza os insumos. As células de dependências de cada exemplo instalam os pacotes específicos de que ele precisa.

O clone utiliza o conteúdo publicado no GitHub. Alterações mantidas apenas no computador local precisam ser publicadas antes de estarem disponíveis em uma nova sessão Colab. Se a sessão já contém um clone antigo, atualize-o antes de executar a preparação.

### Consulta e execução local

Ao usar Jupyter localmente, inicie a sessão dentro deste checkout. A preparação procura a raiz do repositório a partir da pasta atual, inclusive quando o notebook está dentro de uma unidade. Os caminhos dos insumos são construídos a partir dessa raiz, sem depender de pastas pessoais do Google Drive.

O exemplo de processamento de imagem grava `todos.jpg` em `resultados/` da disciplina; essa pasta é criada na execução e fica fora do versionamento. As imagens fornecidas em `dados/imagens/` permanecem como entradas preservadas.

O corpus de tradução conserva o [arquivo de origem e atribuição](disciplinas/processamento-linguagem-natural/dados/traducao/_about.txt). O arquivo GloVe continua disponível apenas localmente ou por obtenção separada, fora do Git.

As saídas já salvas nos notebooks foram preservadas como registros acadêmicos. As adaptações de compatibilidade foram verificadas com testes isolados; a reprodução integral dos exemplos em uma sessão atual do Colab permanece como etapa própria.

### Estado da execução

A revisão de 20/10/2026 corrigiu o gráfico da prática de Pandas e verificou o notebook completo em uma cópia local limpa. As saídas mantidas no acervo continuam históricas. Os 25 notebooks com divergências identificadas trazem um aviso específico no início, sem alterar seus resultados, metadados ou contadores.

A execução integral no Colab e a renovação identificada das saídas permanecem pendentes. O [estado dos 44 notebooks](docs/estado-execucao.md) distingue registros históricos, arquivos sem saídas e a validação local realizada. Os exercícios comentados e as respostas pendentes foram preservados.

### Compatibilidade das bibliotecas

Execute as células na ordem, incluindo as preparações de dependências. KaggleHub usa o extra `pandas-datasets`; Online Retail também prepara `openpyxl` para ler Excel. MovieLens prepara `scikit-surprise==1.1.5`, sem forçar downgrade de NumPy ou encerrar o processo da sessão. Caso uma versão antiga de Surprise já esteja carregada, a célula solicita a reinicialização manual.

Os exemplos iniciais de PLN usam NLTK 3.10.3 e o recurso `punkt_tab`. Os modelos com Keras mantêm a tokenização legada para preservar a lógica dos exercícios; os imports e a declaração das entradas foram atualizados. Os diagramas Seq2Seq verificam pydot e Graphviz: no Colab, a preparação instala Graphviz se ausente; na execução local, o programa `dot` precisa estar no PATH. O exemplo spaCy prepara o modelo português e informa as versões carregadas.

O Atari prepara Gymnasium 1.4.0 e ALE 0.12.1, registra o ambiente original e usa a API de empilhamento atual. Os exemplos de K-Means passam a declarar `n_init` explicitamente; o valor 10 foi adotado nos cinco usos que dependiam do padrão da biblioteca. O modelo final de Online Retail também usa `random_state=42`. Esses ajustes não constituem reprodução dos resultados históricos.

Essas preparações se destinam aos respectivos notebooks; não há exigência de instalar todas as bibliotecas em um único ambiente.

### Fontes automáticas e versões dos dados

As cargas KaggleHub abaixo identificam a versão 1 e validam as colunas essenciais antes do processamento. A conferência dos recursos foi realizada em 2026-10-19.

| Recurso | Handle KaggleHub | Arquivo e recorte |
| --- | --- | --- |
| IMDb | `lakshmi25npathi/imdb-dataset-of-50k-movie-reviews/versions/1` | `IMDB Dataset.csv`, nas 16 práticas de classificação e representação de resenhas de PLN |
| Online Retail | `lakshmi25npathi/online-retail-dataset/versions/1` | `online_retail_II.xlsx`, aba explícita `Year 2009-2010` |
| MovieLens | `snehal1409/movielens/versions/1` | `ratings.csv`, IDs inteiros e notas de 0,5 a 5 |

O CSV IMDb anteriormente carregado pelo Drive foi comparado integralmente com o arquivo Kaggle: os bytes e a ordem das 50.000 linhas são iguais. As 16 cargas usam agora a mesma versão Kaggle; a troca de origem preserva as linhas, inclusive duplicatas. Isso identifica o conteúdo observado, sem garantir a disponibilidade futura dos serviços. Esses arquivos continuam sendo obtidos pelo código e não foram incorporados a `dados/`.

SHA-256 dos recursos conferidos, após extração quando distribuídos em ZIP:

- IMDb CSV: `dfc447764f82be365fa9c2beef4e8df89d3919e3da95f5088004797d79695aa2`.
- Online Retail XLSX: `bcbe73b35f5b7babf197fb0cb983a11f5d9ff929078d4aa53d171b1f2df2e980`.
- MovieLens CSV: `821795331fd974bbe7a8416f2a7eec2b548a485dedb47a073580b0a9a8a0a8d2`.

No MovieLens, os dois Reader declaram a escala de 0,5 a 5, o modelo final recebe todos os parâmetros selecionados por RMSE e a consulta ilustrativa usa IDs inteiros conhecidos. As saídas salvas permanecem históricas; novas previsões e métricas dependem de uma nova execução.

### Nomes e exploração de GloVe

Os catálogos usam nomes que correspondem ao código: regressão com Lasso/Ridge/ElasticNet, a variante de classificação Bag-of-Words com stemming e LSTM com embedding treinável. As renomeações não acrescentam experimentos ao acervo.

Nos cinco notebooks com exploração opcional de GloVe, o classificador aprende embeddings próprios de 128 dimensões. Para executar a exploração, forneça o arquivo indicado, altere `EXPLORAR_GLOVE` para `True` na preparação e execute novamente as células correspondentes. Isso não transfere os vetores para esses modelos. As três integrações efetivas de GloVe continuam documentadas no catálogo de PLN e no README dos vetores.
