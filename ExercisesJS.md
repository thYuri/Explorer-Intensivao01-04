# Exercicios JS

### 1. Crie um script que exiba a mensagem "Hello World!" em um alerta no navegador."
```js
alert ('Hello World!')
```
--- 
<br>

### 2. Crie um script que declare duas variáveis e exiba o resultado da soma entre elas.
```js
const sum = function(number1, number2) {
  alert(number1 + number2)
}
sum(16, 17)

// ou 
let myNumberOne = 16
let myNumberTwo = 17

const soma = myNumberOne + myNumberTwo

// Exibindo no console
console.log('A soma dos números registrados é de: ' + soma)

// Exibindo na caixa de alerta
alert('A soma dos números registrados é de: ' + soma)
```
--- 
<br>

### 3. Crie um script que declare uma variável e verifique se o seu valor é um número. Se for, exiba a mensagem "É um número", caso contrário, exiba a mensagem "Não é um número".
💡 Para saber o tipo de dado você pode usar o operador `typeof`
```js
let myValue = "12345"

// exemplo 1 false: "Não é um número"
if (typeof myValue === 'number') {
  alert("É um número")
} 
else {
  alert("Não é um número")
}

// exemplo 2 true: "É um número"
if (!isNaN(myValue)) {
  alert("É um número")
} 
else {
  alert("Não é um número")
}
// esta função tem um funcionamento diferente e retorna "É um número" porque "12345" é de fato uma string mas ela considera que pode ser transformada em um number
```
--- 
<br>

### 4. Crie um script que declare uma variável e verifique se o seu valor é uma string. Se for, exiba a mensagem "É uma string", caso contrário, exiba a mensagem "Não é uma string".
```js
let myText = "12345"

if (typeof myText === 'string') {
  alert("É uma string")
} 
else {
  alert("Não é uma string")
}
// "12345" entre as aspas é sim uma string portanto retorna true
```
--- 
<br>

### 5. Crie um script que declare uma variável e verifique se o seu valor é um booleano. Se for, exiba a mensagem "É um booleano", caso contrário, exiba a mensagem "Não é um booleano".
```js
let myText = false

if (typeof myText === 'boolean') {
  alert("True. É um booleano")
} 
else {
  alert("False. Não é um booleano")
}
// retorna ("True. É um booleano") 
```
--- 
<br>

### 6. Crie um script que declare duas variáveis e exiba o resultado da subtração entre elas.
```js
// forma 1:
let myNumberOne = Number(16)
let myNumberTwo = Number(7)

const subtraction = (myNumberOne - myNumberTwo)

alert('A subtração dos números registrados é de: ' + subtraction)


// forma 2:
const subtraction = function(number1, number2) {
  alert(number1 - number2)
}
subtraction(16, 7)
```
--- 
<br>

### 7. Crie um script que declare duas variáveis e exiba o resultado da multiplicação entre elas.
```js
const multi = function(number1, number2) {
  alert(number1 * number2)
}

multi(10, 6)
```
--- 
<br>

### 8. Crie um script que declare duas variáveis e exiba o resultado da divisão entre elas.
```js
let number1 = 22
let number2 = 2

const divi = (number1 / number2)

alert(divi)
```
--- 
<br>

### 9. Crie um script que declare uma variável e verifique se o seu valor é um número par. Se for, exiba a mensagem "É um número par", caso contrário, exiba a mensagem "Não é um número par".
```js
let userNumber = prompt('Digite um número:');

// utilizei (diferente de) e inverti a ordem
if (userNumber % 2 !== 0) {
  alert('Não é um número par');
} else {
  alert('É um número par');
}
```
---
<br>

### 10. Crie um script que declare uma variável e verifique se o seu valor é um número ímpar. Se for, exiba a mensagem "É um número ímpar", caso contrário, exiba a mensagem "Não é um número ímpar".
```js
// ou melhor, posso fazer logo os 2 utilizando (condicional OU)
let userNumber = prompt('Digite um número:') 

const evenOrOdd = userNumber % 2 === 0 ? 'par' : 'ímpar'

alert('O número ' + userNumber + ' é ' + evenOrOdd + '.')
```
--- 
<br>