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
- variáveis acumuladoras.

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
