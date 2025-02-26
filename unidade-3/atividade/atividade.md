<p align="center">
  <strong>
    Instituto Federal de Educação, Ciência e Tecnologia do Ceará (IFCE) <br>
    Campus Baturité <br>
    Curso Técnico Subsequente em Informática para Internet
  </strong>
</p>

<p align="center">
  <strong>
    Atividade da Unidade 3 da Disciplina de Lógica de Programação
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

**1. Escreva um algoritmo que receba dois números e retorne a soma, a subtração, a multiplicação e a divisão entre eles**

```js
let numero1 = Number(prompt("Digite um número: "));
let numero2 = Number(prompt("Digite outro número: "));

function fazOperacoesBasicas(num1, num2) {
  alert(`A soma entre ${num1} e ${num2} é igual a: ${num1 + num2}`);
  alert(`A subtração entre ${num1} e ${num2} é igual a: ${num1 - num2}`);
  alert(`A multiplicação entre ${num1} e ${num2} é igual a: ${num1 * num2}`);
  alert(`A divisão entre ${num1} e ${num2} é igual a: ${num1 / num2}`);
}

fazOperacoesBasicas(numero1, numero2);
```

**2. Escreva um algoritmo que receba a base e a altura de um triângulo, calcule e exiba sua área**

```js
let baseDoTriangulo = Number(prompt("Digite a base do triângulo: "));
let alturaDoTriangulo = Number(prompt("Digite a altura do triângulo: "));

function calculaAreaDoTriangulo(base, altura) {
  let areaDoTriangulo = (base * altura) / 2;
  alert(`A área do triângulo é: ${areaDoTriangulo}`);
}

calculaAreaDoTriangulo(baseDoTriangulo, alturaDoTriangulo);
```

**3. Faça um Programa que pergunte quanto você ganha por hora e o número de horas trabalhadas no mês. Calcule e mostre o total do seu salário no referido mês**

```js
let valorQueGanhaPorHora = Number(
  prompt("Digite quanto você ganha por hora: ")
);
let numeroDeHorasTrabalhadasNoMes = Number(
  prompt("Digite o número de horas que você trabalhou nesse mês: ")
);

function calcularSalario(valorPorHora, horasTrabalhadas) {
  let salario = valorPorHora * horasTrabalhadas;
  alert(`Seu salário é: R$${salario}`);
}

calcularSalario(valorQueGanhaPorHora, numeroDeHorasTrabalhadasNoMes);
```

**4. Escreva um programa que peça ao usuário para digitar a sua idade e imprima na tela o número de dias que ele viveu até o momento**

```js
let idade = Number(prompt("Digite a sua idade: "));

function calculaDiasDeVida(idade) {
  let diasVividos = idade * 365;
  alert(`Você já viveu aproximadamente ${diasVividos} dias.`);
}

calculaDiasDeVida(idade);
```

**5. Escreva um programa que peça ao usuário para digitar seu nome e sobrenome separadamente e imprima na tela o nome completo**

```js
let nome = prompt("Digite seu nome: ");
let sobrenome = prompt("Digite seu sobrenome: ");

function imprimeNomeCompleto(nome, sobrenome) {
  alert(`Seu nome completo é: ${nome} ${sobrenome}`);
}

imprimeNomeCompleto(nome, sobrenome);
```

**6. Escreva um programa que peça ao usuário para digitar a temperatura em Celsius e converta para Fahrenheit, imprimindo o resultado na tela**

Resposta:

```js
let temperaturaEmCelsius = Number(prompt("Digite a temperatura em Celsius: "));

function converteTemperaturaParaFahrenheit(temperaturaEmCelsius) {
  let temperaturaEmFahrenheit = (temperaturaEmCelsius * 9) / 5 + 32;
  alert(
    `${temperaturaEmCelsius}°C é equivalente a ${temperaturaEmFahrenheit}°F`
  );
}

converteTemperaturaParaFahrenheit(temperaturaEmCelsius);
```
