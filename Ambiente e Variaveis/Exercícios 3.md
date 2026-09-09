# Exercícios de JavaScript

## Instruções gerais

Resolva os exercícios abaixo em JavaScript.

Para cada questão:

1. Leia atentamente o enunciado e os exemplos.
2. Não altere o nome da função.
3. Não altere os parâmetros recebidos.
4. Implemente sua solução apenas dentro da função.
5. Utilize `return` para devolver o resultado.
6. Teste seu código com os casos apresentados.
7. Sua solução deve funcionar também para outros valores válidos.

---

# Questão 1 — Evolução de energia

## O que você deve fazer

Um personagem inicia seu treinamento com uma determinada quantidade de energia.

A cada dia de treino, sua energia dobra.

Sua função receberá dois valores:

- `energiaInicial`: quantidade de energia no início;
- `dias`: quantidade de dias de treinamento.

A função deve retornar a quantidade de energia após todos os dias de treino.

## Caso 1

**Entrada:**

```js
energiaInicial = 50
dias = 4
```

**Saída esperada:**

```js
800
```

**Explicação:**

A energia evolui da seguinte forma:

```text
50 → 100 → 200 → 400 → 800
```

Após 4 dias, o resultado é `800`.

## Caso 2

**Entrada:**

```js
energiaInicial = 0
dias = 5
```

**Saída esperada:**

```js
0
```

**Explicação:** Dobrar o valor `0` continuará resultando em `0`.

## Caso 3

**Entrada:**

```js
energiaInicial = 25
dias = 0
```

**Saída esperada:**

```js
25
```

**Explicação:** Como nenhum dia de treino ocorreu, o valor permanece igual ao inicial.

## Regras

- `energiaInicial` será do tipo `number`.
- `dias` será um número inteiro.
- `energiaInicial` será maior ou igual a `0`.
- `dias` será maior ou igual a `0`.
- A energia deve dobrar uma vez para cada dia de treino.
- A função deve retornar um `number`.

## Código inicial

```js
function calcularEnergia(energiaInicial, dias) {

}
```

## Para resolver

Você precisará lembrar de:

- funções;
- parâmetros;
- variáveis;
- estruturas de repetição;
- multiplicação;
- variável acumuladora;
- `return`.

---

# Questão 2 — Sequência regressiva

## O que você deve fazer

Sua função receberá um número inteiro chamado `numeroInicial`.

Você deverá produzir uma contagem regressiva começando nesse número e terminando em `0`.

Os números devem ser unidos em uma única `string`, separados pelo caractere `>`.

Caso o valor recebido seja negativo, a função deve retornar:

```text
Valor inválido
```

## Caso 1

**Entrada:**

```js
numeroInicial = 4
```

**Saída esperada:**

```js
'4>3>2>1>0'
```

## Caso 2

**Entrada:**

```js
numeroInicial = 0
```

**Saída esperada:**

```js
'0'
```

## Caso 3

**Entrada:**

```js
numeroInicial = -2
```

**Saída esperada:**

```js
'Valor inválido'
```

## Regras

- `numeroInicial` será um número inteiro.
- Se `numeroInicial < 0`, retorne `'Valor inválido'`.
- Se `numeroInicial === 0`, retorne `'0'`.
- Caso contrário, faça a contagem até `0`.
- Os números devem ser separados por `>`.
- Não deve existir `>` depois do último número.
- Utilize uma estrutura de repetição para montar o resultado.
- O retorno deve ser uma `string`.

## Código inicial

```js
function gerarContagem(numeroInicial) {

}
```

## Para resolver

Você precisará lembrar de:

- `if`;
- estruturas de repetição;
- concatenação de strings;
- conversão de número para texto;
- decremento;
- `return`.

---

# Questão 3 — Produto sequencial

## O que você deve fazer

Implemente uma função que calcule o produto de um número inteiro positivo por todos os inteiros positivos menores que ele até chegar em `1`.

Esse cálculo é conhecido como **fatorial**.

Por exemplo:

```text
5! = 5 × 4 × 3 × 2 × 1
```

Se o valor recebido for negativo, a função deverá retornar:

```text
Valor inválido
```

Para `0`, o resultado deve ser `1`.

## Caso 1

**Entrada:**

```js
n = 6
```

**Saída esperada:**

```js
720
```

**Explicação:**

```text
6 × 5 × 4 × 3 × 2 × 1 = 720
```

## Caso 2

**Entrada:**

```js
n = 0
```

**Saída esperada:**

```js
1
```

**Explicação:** Por definição matemática, `0! = 1`.

## Caso 3

**Entrada:**

```js
n = -4
```

**Saída esperada:**

```js
'Valor inválido'
```

## Caso 4

**Entrada:**

```js
n = 1000000
```

**Saída esperada:**

```js
Infinity
```

**Explicação:** O resultado é grande demais para ser representado normalmente pelo tipo `number` do JavaScript.

## Regras

- `n` será um número inteiro.
- Não utilize recursão.
- Se `n < 0`, retorne `'Valor inválido'`.
- Se `n === 0`, retorne `1`.
- Para valores positivos, calcule o fatorial utilizando repetição.
- O retorno poderá ser:
  - um `number`;
  - `Infinity`;
  - a `string` `'Valor inválido'`.

## Código inicial

```js
function calcularProdutoSequencial(n) {

}
```

## Para resolver

Você precisará lembrar de:

- estruturas condicionais;
- estruturas de repetição;
- multiplicação;
- variável acumuladora;
- decremento;
- `Infinity`;
- `return`.

---

# Conteúdos trabalhados

Estes exercícios trabalham principalmente:

- funções;
- parâmetros;
- `return`;
- variáveis;
- estruturas condicionais;
- estruturas de repetição;
- operadores aritméticos;
- concatenação de strings;
- conversão entre `number` e `string`;
- acumuladores;
- decremento;
- validação de valores;
- fatorial.

---

# Antes de entregar

Confira se:

- [ ] os nomes das funções foram mantidos;
- [ ] os parâmetros não foram alterados;
- [ ] todas as funções retornam algum valor;
- [ ] os exemplos apresentados funcionam;
- [ ] sua solução funciona para outros valores válidos;
- [ ] não há erros de sintaxe;
- [ ] você utilizou `return` em vez de apenas `console.log()`;
- [ ] a Questão 3 foi resolvida sem recursão.
