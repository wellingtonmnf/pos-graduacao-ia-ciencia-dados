# Insumos de Processamento de Linguagem Natural

Esta pasta reúne os arquivos de entrada utilizados manualmente pelos exemplos acadêmicos.

| Pasta | Conteúdo e disponibilidade |
| --- | --- |
| [glove/](glove/README.md) | Instruções para obter os vetores GloVe. O arquivo de vetores é manual e fica fora do Git. |
| [traducao/](traducao/README.md) | Corpus inglês/português por.txt, arquivo compactado original e atribuições preservadas. |

Os notebooks que utilizam esses arquivos definem DATA_DIR na preparação da sessão e validam o insumo necessário. No Colab, o repositório é clonado apenas se ainda não existir na sessão; clones existentes precisam ser atualizados pelo usuário. O envio de GloVe deve ser feito para a cópia do repositório dessa sessão, pois o clone não inclui seus vetores.

Resenhas IMDb, corpora do NLTK e modelos obtidos diretamente por bibliotecas continuam utilizando seus mecanismos originais de acesso. Seus downloads, caches, logs e resultados não foram incorporados a esta pasta.

[Voltar à disciplina](../README.md)
