<p align="center">
  <strong>
    Instituto Federal de Educação, Ciência e Tecnologia do Ceará (IFCE) <br>
    Campus Baturité <br>
    Curso Técnico Subsequente em Informática para Internet
  </strong>
</p>

<p align="center">
  <strong>
    Avaliação II da Disciplina de Lógica de Programação
  </strong>
</p>

<p align="center">
  <strong>
    Baturité-CE <br>
    2024
  </strong>
</p>

<p align="center">
  <strong>
    Identificação do Aluno
  </strong>
</p>

**Nome:** Pedro Henrique Marinho Euzebio
**Professor(a):** Jefferson Lourenço Gurguri
**Curso:** Técnico Subsequente em Informática para Internet
**Turma:** 2024.1

## Objetivo

Desenvolver a habilidade de transformar problemas do mundo real em soluções computacionais através da criação de algoritmos eficientes

## **Materiais**

- **Lista de exercícios:** Fornecida pelo professor, contendo uma série de problemas a serem resolvidos por meio da programação
- **Papel e caneta:** Para a descrição dos pseudocódigos
- **Linguagem de programação:** Escolhida pelo professor ou pelo aluno (ex: Python, C++, Java, etc.)
- **Ambiente de desenvolvimento:** Um editor de código e um compilador/interpretador compatível com a linguagem escolhida

## Instruções

- Desenvolva e descreva algoritmos para os problemas descritos a seguir, as descrições
  dos algoritmos podem ser realizadas utilizando pseudocódigo ou a linguagem de
  programação que desejar
- Esta avaliação consta de 6 items, nomeadamente:
  - Exercício 1.1
  - Exercício 1.2
  - Exercício 2.1
  - Exercício 2.2
  - Exercício 3.1
  - Exercício 3.2
- A prova tem valor total de 12 pontos, sendo pontuado para critério de Prova, no máximo
  10 pontos. Ou seja, temos um item extra (2 pts) extras
- Verifique o número de páginas. A prova contém com 4 páginas, contando com essa

## Parte 1: Estrutura Sequencial

### Exercício 1.1

- No contexto de desenvolvimento de um software para o Caixa (Ponto de Venda) de um
  estabelecimento comercial
- Elabore um algoritmo para capturar os dados de 5 (cinco lançamentos) lançamentos de compra, cada lançamento é composto por um código de identificação de um produto, a quantidade do produto e o valor unitário de cada produto, ao final, calcule e mostre o valor a ser pago

**Exemplo**

| Entrada   | **Saída**              |
| --------- | ---------------------- |
| 12 1 5.30 | Valor a pagar R$ 15.50 |
| 16 2 5.10 |                        |

### Exercício 1.2

- Faça um programa para ler o valor do raio de um círculo, e depois mostrar o valor da área
  deste círculo com quatro casas decimais conforme exemplos
- Fórmula: Area=π∗raio2
- Considere o valor de π=3.141592

**Exemplo**

| Entrada | **Saída**    |
| ------- | ------------ |
| 100.64  | A=31819.3103 |

## Parte 2: Estrutura Condicional

### Exercício 2.1

- Com base na tabela de preços abaixo, faça um programa que leia o código de um item e a
  quantidade deste item
- A seguir, calcule e mostre o valor da conta a pagar

| Código | Especificação   | Preço1 |
| ------ | --------------- | ------ |
| 1      | Cachorro Quente | R$4.00 |
| 2      | X-Salada        | R$4.50 |
| 3      | X-Bacon         | R$5.00 |
| 4      | Torrada simples | R$2.00 |
| 5      | Refrigerante    | R$1.50 |

**Exemplo**

| Entrada | **Saída**      |
| ------- | -------------- |
| 3 2     | Total: R$10.00 |

### Exercício 2.2

- Ler os valores dos três coeficientes "a", "b" e "c" de uma equação do segundo grau
  (ax²+bx+c=0)
- Em seguida, mostrar os valores das raízes da equação, conforme exemplos, usando a fórmula de Baskara (veja abaixo)
- Se a equação não possuir raízes (o valor de "a" não pode ser zero, e o valor de "delta" não pode ser negativo), mostrar uma mensagem "Impossível calcular"
- Fórmula: x=−b±√Δ2a
- Onde: Δ=b2−4ac

**Exemplo**

| Entrada       | **Saída**     |
| ------------- | ------------- |
| 10.0 20.1 5.1 | x1 = -0.29788 |

| Entrada      | **Saída**           |
| ------------ | ------------------- |
| 0.0.20.0.5.0 | Impossível calcular |

## Parte 3: Estrutura de Repetitivas

### Exercício 3.1

- Escreva um algoritmo que repita a leitura de um senha até que ela seja válida
- Para cada leitura de senha incorreta informada, escrever a mensagem "Senha Invalida"
- Quando a senha for confirmada corretamente deve ser impressa a mensagem "Acesso Permitido" e o algoritmo encerrado
- Considere que a senha correta é o valor 2002

| Entrada | **Saída**           |
| ------- | ------------------- |
| 2200    | Impossível calcular |
| 2002    | Acesso Permitido    |

### Exercício 3.2

- Leia um valor inteiro N
- Este valor será a quantidade de valores inteiros X que serão lidos em seguida
- Mostre quantos destes valores X estão dentro do intervalo [10,20] e quando estão fora do intervalo, mostrando essas informações conforme exemplo (use a palavra "in" para dentro do intervalo, e "out" para fora do intervalo)

| Entrada | **Saída** |
| ------- | --------- |
| 5       | 2 in      |
| 14      | 3 out     |
