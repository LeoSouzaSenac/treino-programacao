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
- estrutura condicional `if`.

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
