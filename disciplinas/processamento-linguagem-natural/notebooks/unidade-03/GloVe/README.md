# GloVe — Vetores pré-treinados

Esta pasta é utilizada pelos notebooks desta disciplina que dependem dos vetores pré-treinados **GloVe (Global Vectors for Word Representation)**.

O arquivo utilizado pelos notebooks é:

```text
glove.6B.50d.txt
```

Esse arquivo **não é armazenado neste repositório Git**, pois possui aproximadamente 163 MB e ultrapassa o limite de 100 MB por arquivo do GitHub para repositórios Git convencionais.

As instruções abaixo descrevem a obtenção do arquivo de vetores. Os caminhos e a compatibilidade das bibliotecas de cada notebook ainda precisam ser verificados antes da execução.

---

## 1. Baixar os vetores GloVe

Acesse a página oficial do projeto GloVe da Stanford NLP:

```text
https://nlp.stanford.edu/projects/glove/
```

Baixe o conjunto:

```text
glove.6B.zip
```

Esse pacote contém vetores pré-treinados com diferentes dimensionalidades.

---

## 2. Extrair o arquivo compactado

Após o download, extraia o conteúdo de:

```text
glove.6B.zip
```

O pacote contém os seguintes arquivos:

```text
glove.6B.50d.txt
glove.6B.100d.txt
glove.6B.200d.txt
glove.6B.300d.txt
```

Para os notebooks deste repositório, utilize:

```text
glove.6B.50d.txt
```

---

## 3. Copiar o arquivo para este diretório

Copie:

```text
glove.6B.50d.txt
```

para:

```text
disciplinas/processamento-linguagem-natural/notebooks/unidade-03/GloVe/
```

A estrutura esperada deve ficar assim:

```text
GloVe/
├── README.md
└── glove.6B.50d.txt
```

---

## 4. Verificar o nome do arquivo

O nome deve permanecer exatamente:

```text
glove.6B.50d.txt
```

Não renomeie o arquivo, pois os notebooks podem utilizar esse caminho diretamente no código.

---

## 5. Executar os notebooks

Após obter o arquivo, confira o caminho de leitura no notebook escolhido. Alguns exemplos preservam caminhos do Google Drive; a presença do arquivo nesta pasta, por si só, não garante sua localização pelo código nem a execução do notebook.

Caso ocorra um erro como:

```text
FileNotFoundError
```

verifique:

1. se o arquivo foi extraído do `.zip`;
2. se o arquivo utilizado é `glove.6B.50d.txt`;
3. se ele está dentro da pasta `GloVe`;
4. se o nome e a capitalização do diretório correspondem ao caminho utilizado pelo notebook.

---

## Importante sobre o Git

O arquivo:

```text
glove.6B.50d.txt
```

é mantido apenas localmente e está excluído do versionamento por meio do `.gitignore`.

Não utilize:

```bash
git add -f glove.6B.50d.txt
```

para adicioná-lo ao repositório.

A ausência do arquivo no GitHub é intencional e não representa um arquivo ausente ou erro no repositório.

---

## Referência

**GloVe: Global Vectors for Word Representation**

Jeffrey Pennington, Richard Socher e Christopher D. Manning  
Stanford University

Projeto oficial:

```text
https://nlp.stanford.edu/projects/glove/
```
