# JavaScript Básico

## Exibindo informações

O comando `console.log` é usado para exibir qualquer tipo de informação no console. Por exemplo:

```js
console.log("Matheus Alencar");
console.log(123456);
console.log(3.1415);
// saída:
// Matheus Alencar
// 123456
// 3.1415
```

Podemos representar valores de textos de três forma diferentes, com aspas simples, com aspas duplas e com crase:

```js
console.log('Matheus "Alencar"');
console.log("Matheus 'Alencar'");
console.log(`"Matheus" 'Alencar'`);
// saída:
// Matheus "Alencar"
// Matheus 'Alencar'
// "Matheus" 'Alencar"
```

O comando `console.log` pode receber vários valores separados por vírgula, dessa forma, os valores será exibidos em uma mesma linha separados por um espaço em branco:

```js
console.log("Matheus Alencar", 123456, 3.1415);
// saída:
// Matheus Alencar 123456 3.1415
```

Valores literalmente digitados no código são conhecidos como valores literais.

## Comentários

Comentários são trechos de código que são ignorados pelo motor do JavaScript. Geralmente são usados para fazer anotações no código, com o objetivo de documentar ou explicar algum trecho do código.

```js
// comentário
console.log("Olá mundo!"); // outro comentário
/*
Comentário em bloco 1
Comentário em bloco 2
*/
```

## Variáveis e constantes

São formas de armazenar valores na memória do computador.

### Variáveis

É uma forma de armazenar um valor que pode ser alterado. Existem duas formas de declarar variáveis no JavaScript, usando as palavras reservadas `let` ou `var`, seguidas de um identificador, que seria um nome para a variável:

```js
let nome;
var sobrenome;
```

O termo `var` é mais antigo, então é mais recomendado usar o `let`.

A variável pode ser declarada e já ser inicializada junto com sua declaração, como também pode ser inicializada posteriormente a sua declaração:

```js
let nome = "Matheus";
let sobrenome;
sobrenome = "Alencar";
```

Quando um variável é declarada mas não é inicializada ela tem o valor `undefined`.

Usando uma variável:

```js
let nome = "Matheus";
console.log("Olá ", nome);
// saída:
// Olá  Matheus
```

Existem algumas regras relacionadas a nomemclatura das variáveis no JavaScript:

- Variáveis não podem ter nomes iguais as palavras reservadas da linguagem, as palavras reservadas do JavaScript podem ser encontradas [aqui](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Lexical_grammar#palavras-chave);
- O nome das variáveis não podem começar com números;
- O nome das variáveis também não podem conter espaços em branco ou traços (`-`). No JavaScript se recomenda usar o camelCase, por exemplo `nomeCompleto`;
- As variáveis no JavaScript são case sensitive, ou seja, nomes com caracteres maiúsculas ou minúsculas são consideradas diferentes, por exemplo `nomeCompleto` é diferente de `nomecompleto`.

### Constantes

Também é uma forma de armazenar valores, porém, diferentes das variáveis, as constantes não podem ter seu valores alterados. Elas devem ser declaradas e já inicializadas, usando a palavra reservada `const`.

```js
const nome = "Matheus";
```

As regras relacionadas a nomenclatura das constantes são semelhantes as regras das variáveis.

### `let` x `var`

Variáveis declaradas com `var` podem ser redeclaradas, por exemplo:

```js
var nome = "Matheus";
var nome = "Alencar";
```

Ao tentar fazer essa redeclaração usando `let` um erro será lançado.

## Tipos de dados primitivos

- `string`: caractere ou cadeia de carecteres que representam um valor textual;
- `number`: valores numéricos tanto inteiros como reais (ponto flutuante);
- `undefined`: quando declaramos uma variável mas não atribuimos nenhum valor, ela recebe o valor `undefined`, que não aponta para nenhum local na memeória;
- `null`: é um valor nulo, e também não aponta para nenhum local na memória. Usamos o `null` quando queremos indicar, de forma explícita, que uma variável não deve ter valor, que ela não deve apontar para nenhum lugar na memória. O valor `undefined` não deve ser usado explicitamente pelo programador, ele deve ser deixado para uso somente da própria linguagem JavaScript.
- `booleano`: só pode assumir dois possiveis valores, `true` e `false`, ou seja, verdadeiro e falso.
