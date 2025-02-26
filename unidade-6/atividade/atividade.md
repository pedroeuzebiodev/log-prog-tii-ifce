<p align="center">
  <strong>
    Instituto Federal de Educação, Ciência e Tecnologia do Ceará (IFCE) <br>
    Campus Baturité <br>
    Curso Técnico Subsequente em Informática para Internet
  </strong>
</p>

<p align="center">
  <strong>
    Atividade da Unidade 6 da Disciplina de Lógica de Programação
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

**1. Escreva um programa que crie uma matriz 3x3 com os valores de 1 a 9 e imprima seus valores**

```js
function criaMatriz3Por3() {
  let matriz = [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9],
  ];

  for (let i = 0; i < 3; i++) {
    console.log(matriz[i]);
  }
}

criaMatriz3Por3();
```

**2. Escreva um programa que leia uma matriz 2x2 de valores inteiros informados pelo usuário e imprima sua transposta**

```js
function transpostaMatriz2Por2() {
  let matriz = [];

  for (let i = 0; i < 2; i++) {
    matriz[i] = [];
    for (let j = 0; j < 2; j++) {
      matriz[i][j] = parseInt(
        prompt(`Digite o valor para a posição [${i}][${j}] da matriz: `)
      );
    }
  }

  console.log("Matriz original:");
  console.log(matriz[0]);
  console.log(matriz[1]);

  let transposta = [
    [matriz[0][0], matriz[1][0]],
    [matriz[0][1], matriz[1][1]],
  ];

  console.log("Matriz transposta:");
  console.log(transposta[0]);
  console.log(transposta[1]);
}

transpostaMatriz2Por2();
```

**3. Escreva um programa que leia duas matrizes 3x3 de valores inteiros informadas pelo usuário e imprima a soma de seus valores**

```js
function somaMatrizes3Por3() {
  let matriz1 = [];
  let matriz2 = [];

  for (let i = 0; i < 3; i++) {
    matriz1[i] = [];
    for (let j = 0; j < 3; j++) {
      matriz1[i][j] = parseInt(
        prompt(
          `Digite o valor para a posição [${i}][${j}] da primeira matriz: `
        )
      );
    }
  }

  for (let i = 0; i < 3; i++) {
    matriz2[i] = [];
    for (let j = 0; j < 3; j++) {
      matriz2[i][j] = parseInt(
        prompt(`Digite o valor para a posição [${i}][${j}] da segunda matriz: `)
      );
    }
  }

  let matrizSoma = [];
  for (let i = 0; i < 3; i++) {
    matrizSoma[i] = [];
    for (let j = 0; j < 3; j++) {
      matrizSoma[i][j] = matriz1[i][j] + matriz2[i][j];
    }
  }

  console.log("Matriz resultante da soma:");
  for (let i = 0; i < 3; i++) {
    console.log(matrizSoma[i]);
  }
}

somaMatrizes3Por3();
```
