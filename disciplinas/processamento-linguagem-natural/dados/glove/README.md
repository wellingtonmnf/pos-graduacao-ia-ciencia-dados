# GloVe — vetores pré-treinados

Os oito notebooks desta disciplina que referenciam GloVe esperam o arquivo **glove.6B.50d.txt** nesta pasta:

```text
disciplinas/processamento-linguagem-natural/dados/glove/
├── README.md
└── glove.6B.50d.txt    # arquivo manual, ignorado pelo Git
```

## Obtenção e preparação

1. Acesse o [projeto oficial GloVe, da Stanford NLP](https://nlp.stanford.edu/projects/glove/).
2. Baixe o conjunto **glove.6B.zip** e extraia **glove.6B.50d.txt**. Os vetores de outras dimensionalidades não são os usados por estes exemplos.
3. Copie o arquivo, sem renomeá-lo, para esta pasta dentro da cópia do repositório utilizada pela sessão.
4. No Colab, execute a preparação inicial para localizar ou clonar o repositório. Se o arquivo estiver ausente, a mensagem informa seu caminho absoluto; envie o arquivo para esse destino pelo painel de arquivos e execute a preparação novamente.

O arquivo tem aproximadamente 171 MB (163 MiB) e não acompanha o checkout: está excluído pelo .gitignore e ultrapassa o limite de tamanho do GitHub convencional. Não force sua inclusão no Git. Não há download automático nem configuração de Git LFS nesta organização.

## Uso nos exemplos

A célula inicial define GLOVE_PATH = DATA_DIR / "glove" / "glove.6B.50d.txt" e verifica sua presença. As leituras deixam de depender de um Drive pessoal ou da alteração do diretório de trabalho. Essa preparação não verifica a compatibilidade de todas as dependências nem garante a execução integral.

Alguns exemplos carregam ou preparam a matriz de vetores sem aplicá-la ao modelo ativo. A organização dos arquivos preserva essa implementação acadêmica e suas saídas históricas.

## Referência

Jeffrey Pennington, Richard Socher e Christopher D. Manning. **GloVe: Global Vectors for Word Representation**. Stanford University. [Projeto oficial](https://nlp.stanford.edu/projects/glove/).

[Voltar aos insumos](../README.md)
