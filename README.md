# Máquina de Turing Transdutora Conjugadora de Verbos
Trabalho da disciplina de Computabilidade no curso de graduação de Ciência da Computação na Universidade Estadual da Maringá.
O trabalho desenvolvido descreve uma Máquina de Turing transdutora capaz de conjugar verbos regulares no modo indicativo.

# Entradas e Saídas

A entrada é constituída pelo verbo no modo infinitivo, seguido por dois campos que se separam por meio do símbolo de pipe '|', com o primeiro campo armazenando um número de um a seis que representa o tempo verbal da conjugação e o segundo campo armazenando também um número de um a seis que representa o sujeito do discurso que será utilizado.
A Máquina desenvolvida também realiza um processo de formatação simples, de forma que o verbo regular presente na entrada pode possuir letras minúsculas e maiúsculas, enquanto o verbo na saída será cojugado a partir das informações de entrada possuindo sua primeira letra maiúscula e as demais letras minúsculas.

## Tabela de correspondência

|  Num. | Tempo Verbal (Modo Indicativo) | Sujeito do Discurso    |
| :---: | :----------------------------: | :--------------------: |
|   1   | Presente                       | 1ª Pessoa do Singular  |
|   2   | Pretérito Perfeito             | 2ª Pessoa do Singular  |
|   3   | Pretérito Imperfeito           | 3ª Pessoa do Singular  |
|   4   | Pretérito Mais-Que-Perfeito    | 1ª Pessoa do Plural    |
|   5   | Futuro do Presente             | 2ª Pessoa do Plural    |
|   6   | Futuro do Pretérito            | 3ª Pessoa do Plural    |

## Exemplos

| Entrada          | Saída      |
| :--------------: | :--------: |
| Acreditar\|1\|3  | Acredita   |
| receber\|2\|1    | Recebi     |
| sucumBIR\|3\|6   | Sucumbiam  |
| cEssAr\|4\|2     | Cessaras   |
| mOrReR\|5\|4     | Morreremos |
| SUbir\|6\|5      | Subiríeis  |

# Limitações

* A Máquina apenas funciona para verbos regulares, isto é, verbos cujo radical não se altera durante a conjugação;
  - Exemplo: O verbo "Dormir" possui a conjugação "Durmo", porém a Máquina o transformaria em "Dormo".
* A Máquina não cobre verbos que são apenas foneticamente regulares e mudam alguma parte de seu radical na escrita, isto é, verbos que não são estruturalmente regulares;
  - Exemplo: O verbo "Fornecer" possui a conjugação "Forneço", porém a Máquina o transformaria em "Forneco".
* A Máquina não cobre casos em que a conjugação padrão não ocorre;
  - Exemplo: O verbo "Estar" possui a conjugação "Estão", porém a Máquina o transformaria em "Estam".
* A Máquina opera apenas considerando o modo indicativo para os tempos verbais.
  - Os modos imperativo e subjuntivo não são trabalhados.