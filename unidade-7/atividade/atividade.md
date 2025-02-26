<p align="center">
  <strong>
    Instituto Federal de Educação, Ciência e Tecnologia do Ceará (IFCE) <br>
    Campus Baturité <br>
    Curso Técnico Subsequente em Informática para Internet
  </strong>
</p>

<p align="center">
  <strong>
    Atividade da Unidade 7 da Disciplina de Lógica de Programação
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

**1. Escreva uma função que receba uma lista de números e retorne o valor mínimo encontrado**

```js
function encontraValorMinimo(listaDeNumeros) {
  let valorMinimo = listaDeNumeros[0];
  for (let i = 1; i < listaDeNumeros.length; i++) {
    if (listaDeNumeros[i] < valorMinimo) {
      valorMinimo = listaDeNumeros[i];
    }
  }
  return valorMinimo;
}

let listaDeNumeros = [10, 4, 56, 2, 35];
console.log(`O menor número é: ${encontraValorMinimo(listaDeNumeros)}`);
```

**2. Escreva uma função que receba uma lista de números e um valor inteiro n, e retorne uma nova lista com os n primeiros valores da lista original**

```js
function primeirosValoresDaListaOriginal(lista, n) {
  let novaListaDeNumeros = [];
  for (let i = 0; i < n; i++) {
    novaListaDeNumeros.push(lista[i]);
  }
  return novaListaDeNumeros;
}

let listaDeNumeros2 = [10, 20, 30, 40, 50];
console.log(
  `Os primeiros 3 números são: ${primeirosValoresDaListaOriginal(
    listaDeNumeros2,
    3
  )}`
);
```

**3. Crie um programa principal que importe um arquivo de módulo com as funções dos exercícios anteriores e utilize-as para realizar as seguintes operações: calcular a média de uma lista de números, imprimir a tabuada de um número informado pelo usuário e imprimir os valores de uma lista de números que são maiores que um valor informado pelo usuário**

**`funcoes.js:`**

```js
function encontraValorMinimo(lista) {
  let valorMinimo = lista[0];
  for (let i = 1; i < lista.length; i++) {
    if (lista[i] < valorMinimo) {
      valorMinimo = lista[i];
    }
  }
  return valorMinimo;
}

function primeirosValores(lista, n) {
  let novaListaDeValores = [];
  for (let i = 0; i < n; i++) {
    novaListaDeValores.push(lista[i]);
  }
  return novaListaDeValores;
}

function calculaMediaDeUmaLista(lista) {
  let soma = 0;
  for (let i = 0; i < lista.length; i++) {
    soma += lista[i];
  }
  return soma / lista.length;
}

function mostraValoresMaioresQueUmNumero(lista, valor) {
  return lista.filter((num) => num > valor);
}

module.exports = {
  encontraValorMinimo,
  primeirosValores,
  calculaMediaDeUmaLista,
  mostraValoresMaioresQueUmNumero,
};
```

**`main.js:`**

```js
const funcoes = require("./funcoes");

let numeros = [10, 20, 30, 40, 50];
let media = funcoes.calculaMediaDeUmaLista(numeros);
console.log(`A média da lista é: ${media}`);

function imprimiTabuada(numero) {
  for (let i = 1; i <= 10; i++) {
    console.log(`${numero} x ${i} = ${numero * i}`);
  }
}

let numeroDaTabuada = 5;
console.log(`Tabuada de ${numeroDaTabuada}:`);
imprimiTabuada(numeroDaTabuada);

let numerosMaiores = funcoes.mostraValoresMaioresQueUmNumero(numeros, valor);
console.log(`Números maiores que ${valor}: ${numerosMaiores}`);
```
