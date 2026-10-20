# Insumos de Processamento de Linguagem Natural

Esta pasta reúne os arquivos de entrada utilizados manualmente pelos exemplos acadêmicos.

| Pasta | Conteúdo e disponibilidade |
| --- | --- |
| [glove/](glove/README.md) | Instruções para obter os vetores GloVe. O arquivo de vetores é manual e fica fora do Git. |
| [traducao/](traducao/README.md) | Corpus inglês/português por.txt, arquivo compactado original e atribuições preservadas. |

Os notebooks que utilizam esses arquivos definem DATA_DIR na preparação da sessão e validam o insumo necessário. Dos oito notebooks que referenciam GloVe, três aplicam os pesos em pelo menos um modelo e exigem o arquivo; cinco mantêm uma exploração opcional, desativada por padrão com `EXPLORAR_GLOVE = False`, e seus classificadores podem ser executados sem os vetores. A [documentação GloVe](glove/README.md) identifica cada grupo e explica como ativar a exploração. No Colab, o repositório é clonado apenas se ainda não existir na sessão; clones existentes precisam ser atualizados pelo usuário. O envio de GloVe deve ser feito para a cópia do repositório dessa sessão, pois o clone não inclui seus vetores.

As resenhas IMDb são obtidas pelo KaggleHub na versão 1 de `lakshmi25npathi/imdb-dataset-of-50k-movie-reviews`, com o arquivo `IMDB Dataset.csv`, comum às 16 práticas que usam essa base. A equivalência integral com o antigo CSV do Drive foi conferida em 2026-10-19. Corpora do NLTK e modelos obtidos diretamente por bibliotecas continuam utilizando seus mecanismos de acesso. Seus downloads, caches, logs e resultados não foram incorporados a esta pasta.

[Voltar à disciplina](../README.md)
