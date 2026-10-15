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

Todos os notebooks foram trabalhados no Google Colab. Nos exemplos que leem arquivos de `dados/`, as células iniciais de preparação localizam o repositório e definem a pasta da disciplina e `DATA_DIR`. Quando o repositório ainda não está na sessão Colab, a preparação obtém um clone público em `/content/pos-graduacao-ia-ciencia-dados`.

1. Abra o notebook no Colab e execute as células iniciais de preparação.
2. Os arquivos pequenos versionados acompanham o clone. O arquivo GloVe é obtido separadamente, conforme as [orientações de download e localização](disciplinas/processamento-linguagem-natural/dados/glove/README.md).
3. Continue pelas células do exemplo, observando suas instalações e instruções próprias. A preparação dos arquivos não instala nem atualiza as bibliotecas dos exercícios.

O clone utiliza o conteúdo publicado no GitHub. Alterações mantidas apenas no computador local precisam ser publicadas antes de estarem disponíveis em uma nova sessão Colab. Se a sessão já contém um clone antigo, atualize-o antes de executar a preparação.

### Consulta e execução local

Ao usar Jupyter localmente, inicie a sessão dentro deste checkout. A preparação procura a raiz do repositório a partir da pasta atual, inclusive quando o notebook está dentro de uma unidade. Os caminhos dos insumos são construídos a partir dessa raiz, sem depender de pastas pessoais do Google Drive.

O exemplo de processamento de imagem grava `todos.jpg` em `resultados/` da disciplina; essa pasta é criada na execução e fica fora do versionamento. As imagens fornecidas em `dados/imagens/` permanecem como entradas preservadas.

O corpus de tradução conserva o [arquivo de origem e atribuição](disciplinas/processamento-linguagem-natural/dados/traducao/_about.txt). O arquivo GloVe continua disponível apenas localmente ou por obtenção separada, fora do Git.

As saídas já salvas nos notebooks foram preservadas como registros acadêmicos. A reprodução integral dos exemplos e a compatibilidade das dependências ainda não foram validadas.
