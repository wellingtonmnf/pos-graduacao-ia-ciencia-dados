# GloVe — vetores pré-treinados

Oito notebooks desta disciplina referenciam o arquivo **glove.6B.50d.txt**: três aplicam a matriz em pelo menos um modelo e cinco preservam a preparação como exploração opcional. O arquivo deve ficar nesta pasta quando necessário:

```text
disciplinas/processamento-linguagem-natural/dados/glove/
├── README.md
└── glove.6B.50d.txt    # arquivo manual, ignorado pelo Git
```

## Obtenção e preparação

1. Acesse o [projeto oficial GloVe, da Stanford NLP](https://nlp.stanford.edu/projects/glove/).
2. Baixe o conjunto **glove.6B.zip** e extraia **glove.6B.50d.txt**. Os vetores de outras dimensionalidades não são os usados por estes exemplos.
3. Copie o arquivo, sem renomeá-lo, para esta pasta dentro da cópia do repositório utilizada pela sessão.
4. No Colab, execute a preparação inicial para localizar ou clonar o repositório. Nos três exemplos que aplicam os pesos, ou quando a exploração opcional estiver ativada, a preparação informa o caminho absoluto se o arquivo estiver ausente. Envie o arquivo para esse destino pelo painel de arquivos e execute a preparação novamente.

O arquivo tem aproximadamente 171 MB (163 MiB) e não acompanha o checkout: está excluído pelo .gitignore e ultrapassa o limite de tamanho do GitHub convencional. Não force sua inclusão no Git. Não há download automático nem configuração de Git LFS nesta organização.

## Modelos que aplicam os pesos

Estes notebooks exigem o arquivo para o experimento que utiliza a matriz:

- [Classificação com GloVe](../../notebooks/unidade-03/classificacao-com-glove.ipynb): inicializa a camada de embedding com a matriz.
- [CNN — alternativo](../../notebooks/unidade-03/classificacao-com-cnn-alternativo.ipynb): o segundo dos três modelos utiliza a matriz; a afirmação não se estende aos outros modelos.
- [Classificação com LSTM](../../notebooks/unidade-04/classificacao-com-lstm.ipynb): utiliza a matriz com pesos congelados (`trainable=False`).

## Exploração opcional sem integração ao classificador

Os cinco notebooks abaixo utilizam embeddings treináveis de 128 dimensões. A exploração prepara uma matriz GloVe de 50 dimensões, mas não a passa aos modelos ativos:

- [CNN](../../notebooks/unidade-03/classificacao-com-cnn.ipynb).
- [CNN/LSTM](../../notebooks/unidade-04/classificacao-com-cnn-lstm.ipynb).
- [CNN/LSTM com dropout](../../notebooks/unidade-04/classificacao-com-cnn-lstm-dropout.ipynb).
- [LSTM — alternativo](../../notebooks/unidade-04/classificacao-com-lstm-alternativo.ipynb): ambos os modelos ativos utilizam embedding próprio.
- [LSTM com embedding treinável](../../notebooks/unidade-04/classificacao-com-lstm-embedding-treinavel.ipynb).

Neles, a preparação define `EXPLORAR_GLOVE = False`. Assim, o arquivo não é exigido nem lido, e `embedding_matrix` fica como `None`. Para executar a exploração, obtenha e copie o arquivo para o destino acima, altere o controle para `True` e execute novamente a preparação e depois as células exploratórias, na ordem do notebook. Ativar esse controle não muda a arquitetura nem integra os vetores ao classificador. As alternativas de camadas comentadas permanecem inativas.

A célula inicial define `GLOVE_PATH = DATA_DIR / "glove" / "glove.6B.50d.txt"`. As leituras deixam de depender de um Drive pessoal ou da alteração do diretório de trabalho. Essa preparação não verifica a compatibilidade de todas as dependências nem garante a execução integral. As saídas históricas podem mostrar explorações anteriores mesmo com o controle atualmente desativado.

## Referência

Jeffrey Pennington, Richard Socher e Christopher D. Manning. **GloVe: Global Vectors for Word Representation**. Stanford University. [Projeto oficial](https://nlp.stanford.edu/projects/glove/).

[Voltar aos insumos](../README.md)
