# Exercícios de JavaScript

## Instruções gerais

Resolva os três exercícios abaixo utilizando JavaScript.

Para cada questão:

1. Leia o enunciado e observe os exemplos.
2. Não altere o nome da função.
3. Não altere os parâmetros recebidos pela função.
4. Escreva sua solução somente dentro da função fornecida.
5. Utilize `return` para devolver o resultado solicitado.
6. Teste seu código com os exemplos apresentados.
7. Sua solução deve funcionar também para outros valores válidos, não apenas para os exemplos.

---

# Questão 1 — Inverter os algarismos de um número

## O que você deve fazer

Sua função receberá um número inteiro chamado `valor`.

Você deverá inverter a ordem de seus algarismos e retornar o novo número.

Se o número for negativo, o sinal de negativo deverá continuar no início do resultado.

## Caso 1

**Entrada:**

```js
valor = 2481
```

**Saída esperada:**

```js
1842
```

**Explicação:** Os algarismos de `2481` foram invertidos, resultando em `1842`.

## Caso 2

**Entrada:**

```js
valor = 7306
```

**Saída esperada:**

```js
6037
```

**Explicação:** Os algarismos de `7306` foram colocados na ordem inversa.

## Caso 3

**Entrada:**

```js
valor = -425
```

**Saída esperada:**

```js
-524
```

**Explicação:** O número foi invertido, mas continuou sendo negativo.

## Regras

- `valor` será um número inteiro.
- O número poderá ser positivo ou negativo.
- O retorno deve ser do tipo `number`.
- O sinal negativo deve ser mantido quando o número recebido for negativo.

## Código inicial

```js
function inverterAlgarismos(valor) {

}
```

## Para resolver

Você precisará pensar em:

- conversão entre `number` e `string`;
- manipulação de texto;
- inversão da ordem dos caracteres;
- números negativos;
- conversão de volta para `number`;
- uso de `return`.

## Onde estudar

### Funções, parâmetros e `return`

Material didático:

- MDN — Funções:  
  https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Guide/Functions

Leia principalmente sobre:

- declaração de funções;
- parâmetros;
- valores de retorno;
- `return`.

### Tipos `number` e `string`

Material didático:

- MDN — Tipos e estruturas de dados:  
  https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Guide/Data_structures

Você precisa entender principalmente a diferença entre:

```js
123
```

e:

```js
"123"
```

O primeiro é um número e o segundo é um texto.

### Converter número para string

Material:

- MDN — `String()`:  
  https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Global_Objects/String/String

Exemplo:

```js
String(123)
```

Resultado:

```js
"123"
```

### Converter string para número

Material:

- MDN — `Number()`:  
  https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Global_Objects/Number/Number

Exemplo:

```js
Number("123")
```

Resultado:

```js
123
```

### Manipulação de strings

Material didático:

- MDN — Trabalhando com texto:  
  https://developer.mozilla.org/pt-BR/docs/Learn_web_development/Core/Scripting/Strings

Estude principalmente:

- acessar caracteres;
- transformar uma string;
- juntar e separar textos.

### Arrays e `reverse()`

Uma forma de inverter caracteres é transformar o texto em array e depois inverter esse array.

Material:

- MDN — `split()`:  
  https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Global_Objects/String/split

- MDN — `reverse()`:  
  https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Global_Objects/Array/reverse

- MDN — `join()`:  
  https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Global_Objects/Array/join

Esses três métodos costumam aparecer juntos em problemas desse tipo:

```text
string → array → inverter → string
```

### Números negativos

Material:

- MDN — Operadores aritméticos:  
  https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Guide/Expressions_and_operators#operadores_aritm%C3%A9ticos

Você também pode consultar:

- MDN — `Math.abs()`:  
  https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Global_Objects/Math/abs

`Math.abs()` devolve o valor absoluto de um número.

Exemplo:

```js
Math.abs(-25)
```

Resultado:

```js
25
```

---

# Questão 2 — Somar os valores pares

## O que você deve fazer

Sua função receberá um array de números inteiros chamado `valores`.

Você deverá percorrer o array, identificar quais números são pares e retornar a soma de todos eles.

## Caso 1

**Entrada:**

```js
valores = [2, 5, 8, 11, 14]
```

**Saída esperada:**

```js
24
```

**Explicação:** Os números pares são `2`, `8` e `14`. A soma é `24`.

## Caso 2

**Entrada:**

```js
valores = [7, 4, 12, 3, 6]
```

**Saída esperada:**

```js
22
```

**Explicação:** Os números pares são `4`, `12` e `6`.

## Caso 3

**Entrada:**

```js
valores = [10, 13, 20, 9, 2]
```

**Saída esperada:**

```js
32
```

**Explicação:** Os números pares são `10`, `20` e `2`.

## Regras

- `valores` será um array de números inteiros.
- O array terá pelo menos um elemento.
- Cada valor poderá ser positivo ou negativo.
- Considere `0` como um número par.
- O retorno deve ser um `number`.

## Código inicial

```js
function somarValoresPares(valores) {

}
```

## Para resolver

Você precisará lembrar de:

- arrays;
- repetição com `for`, `for...of` ou outra estrutura equivalente;
- operador `%`;
- identificação de números pares;
- variável acumuladora;
- `if`;
- `return`.

## Onde estudar

### Arrays

Material didático:

- MDN — Arrays:  
  https://developer.mozilla.org/pt-BR/docs/Learn_web_development/Core/Scripting/Arrays

Leia principalmente sobre:

- criação de arrays;
- posições;
- elementos;
- `length`;
- como percorrer os valores.

Exemplo:

```js
const numeros = [2, 4, 6]
```

### Estruturas de repetição

Material:

- MDN — Laços e iterações:  
  https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Guide/Loops_and_iteration

Para esta questão, estude principalmente:

```js
for
for...of
```

Exemplo:

```js
for (const numero of numeros) {
    // código executado para cada número
}
```

### Estrutura condicional `if`

Material didático:

- MDN — Condicionais:  
  https://developer.mozilla.org/pt-BR/docs/Learn_web_development/Core/Scripting/Conditionals

Você utilizará uma condição para decidir se determinado número deve ou não entrar na soma.

### Operador módulo `%`

Material:

- MDN — Operador resto `%`:  
  https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Operators/Remainder

O operador `%` informa o resto de uma divisão.

Exemplo:

```js
10 % 2
```

Resultado:

```js
0
```

Isso é útil para identificar números pares.

Uma propriedade importante:

```text
Se um número inteiro dividido por 2 tem resto 0, ele é par.
```

### Comparações

Material:

- MDN — Operadores de comparação:  
  https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Guide/Expressions_and_operators#operadores_de_compara%C3%A7%C3%A3o

Observe principalmente o operador:

```js
===
```

### Variável acumuladora

Uma variável acumuladora guarda um resultado e vai sendo atualizada durante uma repetição.

Exemplo:

```js
let soma = 0

soma = soma + 4
soma = soma + 8
```

Também é possível escrever:

```js
soma += 4
```

Material relacionado:

- MDN — Operadores de atribuição:  
  https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Guide/Expressions_and_operators#operadores_de_atribui%C3%A7%C3%A3o

### `return`

Material:

- MDN — Funções:  
  https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Guide/Functions

Lembre-se: `console.log()` apenas mostra um valor. O exercício pede que a função **retorne** o resultado.

---

# Questão 3 — Somar os valores ímpares

## O que você deve fazer

Sua função receberá um array de números inteiros chamado `numeros`.

Você deverá percorrer esse array, encontrar os valores ímpares e retornar a soma deles.

## Caso 1

**Entrada:**

```js
numeros = [1, 4, 7, 8, 9]
```

**Saída esperada:**

```js
17
```

**Explicação:** Os números ímpares são `1`, `7` e `9`. A soma é `17`.

## Caso 2

**Entrada:**

```js
numeros = [6, 3, 11, 12, 5]
```

**Saída esperada:**

```js
19
```

**Explicação:** Os números ímpares são `3`, `11` e `5`.

## Caso 3

**Entrada:**

```js
numeros = [15, 20, 21, 30]
```

**Saída esperada:**

```js
36
```

**Explicação:** Os números ímpares são `15` e `21`.

## Regras

- `numeros` será um array de números inteiros.
- O array terá pelo menos um elemento.
- Cada elemento poderá ser positivo, negativo ou zero.
- O retorno deve ser um `number`.

## Código inicial

```js
function somarValoresImpares(numeros) {

}
```

## Para resolver

Você precisará lembrar de:

- arrays;
- estruturas de repetição;
- operador `%`;
- diferença entre números pares e ímpares;
- estrutura condicional `if`;
- variável acumuladora;
- `return`.

## Onde estudar

### Arrays

Material didático:

- MDN — Arrays:  
  https://developer.mozilla.org/pt-BR/docs/Learn_web_development/Core/Scripting/Arrays

Concentre-se em:

- elementos;
- posições;
- tamanho do array;
- percorrer todos os elementos.

### Estruturas de repetição

Material:

- MDN — Laços e iterações:  
  https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Guide/Loops_and_iteration

Para este exercício, `for` ou `for...of` são suficientes.

### Operador módulo `%`

Material:

- MDN — Operador resto `%`:  
  https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Operators/Remainder

Para números positivos:

```js
numero % 2
```

retornará:

```js
0
```

quando o número for par.

Para números ímpares, o resultado será diferente de `0`.

Como o exercício também aceita números negativos, compare o resultado com `0`, em vez de assumir que o resto será sempre `1`.

### Operadores de comparação

Material:

- MDN — Operadores de comparação:  
  https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Guide/Expressions_and_operators#operadores_de_compara%C3%A7%C3%A3o

Observe principalmente:

```js
===
!==
```

### Estrutura condicional `if`

Material:

- MDN — Condicionais:  
  https://developer.mozilla.org/pt-BR/docs/Learn_web_development/Core/Scripting/Conditionals

A condição será utilizada para decidir quais números devem ser adicionados à soma.

### Variável acumuladora

Para somar vários valores, você pode começar com:

```js
let soma = 0
```

e atualizar a variável enquanto percorre o array.

Exemplo conceitual:

```js
soma = soma + numero
```

ou:

```js
soma += numero
```

Material:

- MDN — Operadores de atribuição:  
  https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Guide/Expressions_and_operators#operadores_de_atribui%C3%A7%C3%A3o

### Funções e `return`

Material:

- MDN — Funções:  
  https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Guide/Functions

Sua função deve devolver a soma final utilizando `return`.

---

# Conteúdos trabalhados

Estes exercícios trabalham principalmente:

- funções;
- parâmetros;
- `return`;
- tipos de dados;
- conversão entre `number` e `string`;
- manipulação de strings;
- arrays;
- estruturas de repetição;
- estruturas condicionais;
- operador módulo `%`;
- números pares e ímpares;
- operadores de comparação;
- variáveis acumuladoras.

---

# Documentação geral recomendada

## MDN — JavaScript para iniciantes

https://developer.mozilla.org/pt-BR/docs/Learn_web_development/Core/Scripting

Essa parte da documentação é uma das mais indicadas para quem ainda está aprendendo JavaScript. Os conteúdos são apresentados de forma mais didática do que nas páginas de referência técnica.

## Guia de JavaScript da MDN

https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Guide

Use o guia quando precisar revisar um assunto específico, como:

- funções;
- loops;
- operadores;
- tipos de dados;
- objetos;
- arrays.

## Referência JavaScript da MDN

https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference

A referência é útil quando você já sabe o recurso que procura e quer descobrir exatamente como ele funciona.

Por exemplo:

```text
String()
Number()
split()
reverse()
join()
```

---

# Antes de entregar

Confira se:

- [ ] você manteve os nomes das funções;
- [ ] você manteve os parâmetros solicitados;
- [ ] cada função retorna o resultado correto;
- [ ] os exemplos apresentados funcionam;
- [ ] sua solução funciona com outros valores;
- [ ] não existem erros de sintaxe;
- [ ] você não deixou `console.log()` no lugar do `return`.
