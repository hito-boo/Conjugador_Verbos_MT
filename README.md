# conjugador_verbos_MT
Trabalho da disciplina de Computabilidade no curso de graduação de Ciência da Computação na Universidade Estadual da Maringá.
O trabalho desenvolvido descreve uma Máquina de Turing transdutora capaz de conjugar verbos regulares no modo indicativo.

# Entradas e Saídas

A entrada é composta por três campos separados pelo símbolo de Pipe '|'. No primeiro campo, há o verbo regular no infinitivo; no segundo, há um número que representa o tempo verbal que será utilizado para conjugar o verbo; e por fim, no terceiro, há um número que representa o sujeito do discurso que será utilizado na conjugação. A correspondência de números e de sujeitos é dado pelas seguintes tabelas:

## Tabela dos Tempos Verbais (Todos no Modo Indicativo)

|  Num. | Tempo Verbal                   |
| ----- | ------------------------------ |
|   1   |  Presente                      |
|   2   |  Pretérito Perfeito            |
|   3   |  Pretérito Imperfeito          |
|   4   |  Pretérito Mais-Que-Perfeito   |
|   5   |  Futuro do Presente            |
|   6   |  Futuro do Pretérito           |

## Tabela dos Sujeitos

|  Num. | Sujeito do Discurso                |
| ----- | ---------------------------------- |
|   1   |  Primeira do Singular (Eu)         |
|   2   |  Segunda do Singular (Tu)          |
|   3   |  Terceira do Singular (Ele, Ela)   |
|   4   |  Primeira do Plural (Nós)          |
|   5   |  Segunda do Plural (Vós)           |
|   6   |  Terceira do Plural (Eles, Elas)   |

## Exemplos de Entrada

guardar|1|1 -> guardo
amar|2|3 -> amou
