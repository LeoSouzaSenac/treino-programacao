# Exercícios de JavaScript

## Instruções gerais

Para cada exercício:

1. Leia o enunciado e os exemplos antes de começar.
2. Não altere o nome da função.
3. Não altere os nomes dos parâmetros.
4. Escreva sua solução dentro da função fornecida.
5. Use `return` para devolver o resultado solicitado.
6. Teste o código utilizando os exemplos do exercício.
7. A solução deve funcionar para outros valores que respeitem as regras do exercício.

---

# Questão 1 — Criando uma ficha de aluno

## O que você deve fazer

Uma escola precisa organizar algumas informações básicas de seus alunos.

Sua função receberá o **nome** e a **idade** de um aluno. A partir desses dados, crie um objeto contendo as propriedades `nome` e `idade`.

Depois, retorne o objeto criado.

## Caso 1

**Entrada:**

```js
nome = 'Ana'
idade = 18
```

**Saída esperada:**

```js
{ nome: 'Ana', idade: 18 }
```

## Caso 2

**Entrada:**

```js
nome = 'Carlos'
idade = 21
```

**Saída esperada:**

```js
{ nome: 'Carlos', idade: 21 }
```

## Caso 3

**Entrada:**

```js
nome = 'Fernanda'
idade = 16
```

**Saída esperada:**

```js
{ nome: 'Fernanda', idade: 16 }
```

## Regras

- `nome` será uma `string`.
- `idade` será um `number`.
- Os valores recebidos devem ser armazenados em um objeto.
- O objeto deve possuir as propriedades `nome` e `idade`.
- A função deve retornar o objeto criado.

## Código inicial

```js
function criarFichaAluno(nome, idade) {

}
```

## Para resolver

Você precisará lembrar de:

- como criar um objeto em JavaScript;
- como adicionar propriedades e valores em um objeto;
- como utilizar parâmetros de uma função;
- como retornar um valor utilizando `return`.

## Onde estudar

### Objetos em JavaScript

Material didático:

- MDN — Trabalhando com objetos:  
  https://developer.mozilla.org/pt-BR/docs/Learn_web_development/Core/Scripting/Object_basics

Leia principalmente sobre:

- como criar um objeto;
- propriedades;
- valores;
- acesso às propriedades.

Exemplo:

```js
const pessoa = {
    nome: "Ana",
    idade: 18
}
```

### Propriedades de objetos

Material:

- MDN — Trabalhando com objetos:  
  https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Guide/Working_with_objects

Observe principalmente como uma propriedade é formada por uma chave e um valor:

```js
nome: "Ana"
```

### Funções e parâmetros

Material didático:

- MDN — Funções:  
  https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Guide/Functions

Leia principalmente sobre:

- declaração de função;
- parâmetros;
- argumentos;
- valores recebidos pela função.

Exemplo:

```js
function mostrarPessoa(nome, idade) {

}
```

Nesse exemplo, `nome` e `idade` são parâmetros.

### `return`

Material:

- MDN — Funções:  
  https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Guide/Functions

O `return` serve para devolver um valor para quem chamou a função.

Exemplo:

```js
function exemplo() {
    return 10
}
```

---

# Questão 2 — Montando uma mensagem

## O que você deve fazer

Um sistema precisa criar pequenas mensagens utilizando duas partes de texto.

Sua função receberá uma **saudação** e um **nome**.

Você deverá juntar os dois valores colocando **um espaço entre eles** e retornar a mensagem resultante.

## Caso 1

**Entrada:**

```js
saudacao = 'Olá'
nome = 'Carlos'
```

**Saída esperada:**

```js
'Olá Carlos'
```

## Caso 2

**Entrada:**

```js
saudacao = 'Bom dia'
nome = 'Marina'
```

**Saída esperada:**

```js
'Bom dia Marina'
```

## Caso 3

**Entrada:**

```js
saudacao = 'Bem-vindo'
nome = 'Pedro'
```

**Saída esperada:**

```js
'Bem-vindo Pedro'
```

## Regras

- `saudacao` será uma `string`.
- `nome` será uma `string`.
- Deve existir exatamente um espaço entre os dois valores.
- A função deve retornar uma `string`.
- Caso algum dos dois valores seja uma `string` vazia, retorne uma `string` vazia.

## Código inicial

```js
function montarMensagem(saudacao, nome) {

}
```

## Para resolver

Você precisará lembrar de:

- como trabalhar com `string`;
- como juntar textos;
- como colocar um espaço entre dois textos;
- como utilizar `if` para verificar uma condição;
- como utilizar `return`.

Você pode utilizar concatenação com `+` ou template string.

## Onde estudar

### Strings

Material didático:

- MDN — Strings:  
  https://developer.mozilla.org/pt-BR/docs/Learn_web_development/Core/Scripting/Strings

Leia principalmente sobre:

- criação de textos;
- aspas simples e duplas;
- concatenação;
- template strings.

Exemplo:

```js
const nome = "Carlos"
```

### Concatenação de textos

Material:

- MDN — Strings:  
  https://developer.mozilla.org/pt-BR/docs/Learn_web_development/Core/Scripting/Strings

Uma forma de juntar textos é usando `+`.

Exemplo:

```js
"Olá" + " " + "Carlos"
```

Resultado:

```js
"Olá Carlos"
```

### Template strings

Material:

- MDN — Template literals:  
  https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Template_literals

Exemplo:

```js
`${saudacao} ${nome}`
```

Template strings utilizam crase:

```text
`
```

e permitem inserir valores com:

```js
${valor}
```

### Estrutura condicional `if`

Material didático:

- MDN — Condicionais:  
  https://developer.mozilla.org/pt-BR/docs/Learn_web_development/Core/Scripting/Conditionals

Para esta questão, o `if` pode ser utilizado para verificar se algum texto está vazio.

Exemplo:

```js
if (nome === "") {
    // alguma ação
}
```

### Operadores de comparação

Material:

- MDN — Operadores de comparação:  
  https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Guide/Expressions_and_operators#operadores_de_compara%C3%A7%C3%A3o

Observe principalmente:

```js
===
```

### `return`

Material:

- MDN — Funções:  
  https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Guide/Functions

Lembre-se de que:

```js
console.log(resultado)
```

apenas mostra o valor.

Já:

```js
return resultado
```

devolve o valor da função.

---

# Questão 3 — Transformando uma pontuação em texto

## O que você deve fazer

Em algumas situações, um sistema precisa transformar um valor numérico em texto antes de exibi-lo.

Sua função receberá uma pontuação do tipo `number`.

Você deverá converter esse valor para o tipo `string` e retorná-lo.

O valor da pontuação deve continuar sendo o mesmo. Apenas o tipo do dado deve mudar.

## Caso 1

**Entrada:**

```js
pontos = 250
```

**Saída esperada:**

```js
'250'
```

## Caso 2

**Entrada:**

```js
pontos = 0
```

**Saída esperada:**

```js
'0'
```

## Caso 3

**Entrada:**

```js
pontos = 42.5
```

**Saída esperada:**

```js
'42.5'
```

## Caso 4

**Entrada:**

```js
pontos = -10
```

**Saída esperada:**

```js
'-10'
```

## Regras

- `pontos` será do tipo `number`.
- O número pode ser positivo, negativo, decimal ou zero.
- O valor retornado deve ser do tipo `string`.
- A função deve retornar o mesmo valor recebido, apenas convertido para texto.

## Código inicial

```js
function transformarPontuacaoEmTexto(pontos) {

}
```

## Para resolver

Você precisará lembrar de:

- a diferença entre `number` e `string`;
- como verificar o tipo de um valor;
- como converter um número para texto;
- como utilizar `return`.

## Onde estudar

### Tipos de dados

Material didático:

- MDN — Tipos e estruturas de dados:  
  https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Guide/Data_structures

Para esta questão, concentre-se principalmente em:

- `number`;
- `string`.

Compare:

```js
250
```

com:

```js
"250"
```

Eles parecem semelhantes na tela, mas são tipos de dados diferentes.

### `number`

Material:

- MDN — Number:  
  https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Global_Objects/Number

Exemplos de valores do tipo `number`:

```js
10
0
-5
42.5
```

### `string`

Material:

- MDN — Strings:  
  https://developer.mozilla.org/pt-BR/docs/Learn_web_development/Core/Scripting/Strings

Exemplos de strings:

```js
"10"
"Olá"
"-5"
"42.5"
```

### Verificar o tipo com `typeof`

Material:

- MDN — `typeof`:  
  https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Operators/typeof

Exemplo:

```js
typeof 250
```

Resultado:

```js
"number"
```

Exemplo:

```js
typeof "250"
```

Resultado:

```js
"string"
```

### Converter um número para string

Material:

- MDN — `String()`:  
  https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Global_Objects/String/String

Exemplo:

```js
String(250)
```

Resultado:

```js
"250"
```

Observe que o valor continua representando `250`, mas agora é um texto.

### Conversão de tipos

Material complementar:

- MDN — Conversão de tipos:  
  https://developer.mozilla.org/pt-BR/docs/Glossary/Type_Conversion

A conversão de tipos acontece quando um valor passa de um tipo para outro.

Exemplo:

```text
number → string
```

### `return`

Material:

- MDN — Funções:  
  https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Guide/Functions

Depois de converter o valor, a função deve devolvê-lo com `return`.

---

# Conteúdos trabalhados

Os exercícios trabalham principalmente os seguintes conteúdos:

- funções;
- parâmetros;
- `return`;
- tipos de dados;
- `string`;
- `number`;
- objetos;
- propriedades de objetos;
- concatenação de textos;
- template strings;
- conversão de tipos;
- estrutura condicional `if`;
- operador de comparação `===`;
- operador `typeof`.

---

# Documentação geral recomendada

## MDN — JavaScript para iniciantes

https://developer.mozilla.org/pt-BR/docs/Learn_web_development/Core/Scripting

Essa é uma das partes mais indicadas da MDN para quem ainda está começando com JavaScript.

Os conteúdos possuem explicações, exemplos e exercícios.

## Guia de JavaScript da MDN

https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Guide

Use para revisar assuntos como:

- funções;
- objetos;
- tipos;
- operadores;
- estruturas condicionais.

## Referência JavaScript da MDN

https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference

Use quando quiser consultar um recurso específico da linguagem.

Exemplos:

```text
String()
Number()
typeof
return
```

---

# Antes de entregar

Confira se:

- [ ] você não alterou os nomes das funções;
- [ ] você não alterou os parâmetros;
- [ ] todas as funções possuem `return`;
- [ ] os exemplos apresentados funcionam;
- [ ] seu código funciona também com outros valores;
- [ ] não existem erros de sintaxe;
- [ ] você escreveu apenas o necessário dentro de cada função.
