# JavaScript Básico

## Exibindo informações

O comando `console.log` é usado para exibir qualquer tipo de informação no console. Por exemplo:

```js
console.log('Matheus Alencar');
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
console.log('Matheus Alencar', 123456, 3.1415);
// saída:
// Matheus Alencar 123456 3.1415
```

Valores literalmente digitados no código são conhecidos como valores literais.

## Comentários

Comentários são trechos de código que são ignorados pelo motor do JavaScript. Geralmente são usados para fazer anotações no código, com o objetivo de documentar ou explicar algum trecho do código.

```js
// comentário
console.log('Olá mundo!'); // outro comentário
/*
Comentário em bloco 1
Comentário em bloco 2
*/
```