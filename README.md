# Caderno virtual - Lógica da Programação e Algoritmos
Boas vindas! Este é seu caderno virtual. Aqui você deverá guardar todos os conceitos aprendidos e atiuvidades dessa unidade curricular. 


## Conteúdo Técnico
```js
const nome = "Alberto";
console.log(nome);
```
```js
const nome = prompt("lembrete do dia, oque você tem que fazer hoje?");

if (nome == "animar") {
  console.log(`ainda bem que você lembrou, vá ${nome}`);
} else {
  console.log(`não, você não precisa ${nome} hoje.`);
}
```
```js
const produto = prompt("Olá, Qual mangá você desejaria");

switch (produto) {
  case "One Piece":
    console.log("O One Piece custa R$30,00.");
    break;
  case "Jujutsu Kaisen":
    console.log("O Jujutsu Kaisen custa R$24,00.");
    break;
  case "Mob Psycho":
    console.log("o Mob Psycho custa R$25,00.");
    break;
  case "Made in Abyss":
    console.log("O Made in Abyss custa R$24,00.");
    break;
  case "Demon Slayer":
    console.log("O Demon Slayer custa R$22,00.");
    break;
  default:
    console.log("infelizmente não temos esse disponivel");
}
```
```js
// Organizando por critérios (ordem alfabética)
const livros = ["Javascript Assertivo", "Engenharia de Testes", "Clean code", "Scrum", "Guia HTML5 e CSS3", "MongoDB"]

livros.sort();

console.log(livros)

// contando os elementos
console.log(livros.length)

// usando for para lista horizontal
```
```js
const livros = [
  "Javascript Assertivo",
  "Engenharia de Testes",
  "Clean code",
  "Scrum",
  "Guia HTML5 e CSS3",
  "MongoDB"
];

console.log(livros.length); //retorna a quantidade de elementos de um array.

console.log(livros.pop); //remove o último elemento de um array e retorna este elemento.

console.log(livros.push()); //adiciona um ou mais elementos ao final de um array e retorna o tamanho deste array.

console.log(livros.shift()); //remove o primeiro elemento de um array e retorna esse elemento.

console.log(livros.unshift("vue.js")); //adiciona um ou mais elementos no início de um array e retorna o tamanho deste array.

console.log(livros);
```
```js
var frutas = prompt("Qual fruta você deseja?");

var array = [1, 2];
var pos = frutas.indexOf(1); // Maçã
var pos = frutas.indexOf(2); // bananas
var pos = frutas.indexOf(0); // caju

switch (frutas) {
  case "maçã":
    console.log("maçã está 3,50");
    break;
  case "bananas":
    console.log("bananas estão 6,00");
    break;
  case "caju":
    console.log("não temos caju");
    break;
}
```
```js
const livros = [
  "javascript Assertivo",
  "Engenharia de Testes",
  "Clean code",
  "Scrum",
  "Guia HTML5 e CSS3",
  "MongoDB"
];

const atualizandoLivros = livros.splice(0, 0, "Node.Js");
//(indice localização, n de elementos p/ deletar, adicionar)
console.log(atualizandoLivros);

console.log(livros);
```
```js
const livros = [
  "javascript Assertivo",
  "Engenharia de Testes",
  "Clean code",
  "Scrum",
  "Guia HTML5 e CSS3",
  "MongoDB"
];

const tamanhoLivros = livros.length;

const corredorA1 = livros.slice(0, tamanhoLivros / 3);

const corredorA2 = livros.slice(tamanhoLivros / 3);

console.log(`Os livros do corredor A1 são:`, corredorA1);
console.log(`Os livros do corredor A2 são:`, corredorA2);
```
```js
const livros = [
  "javascript Assertivo",
  "Engenharia de Testes",
  "Clean code",
  "Scrum",
  "Guia HTML5 e CSS3",
  "MongoDB"
];

const hqs = ["Batman", "Sonic IDW", "Avatar", "Homem Aranha", "Vingadores"];

const mangá = ["Jujutsu Kaisen", "Mob Psycho", "One Piece", "Punpun"];

const JuntarLivros = livros.concat(hqs, mangá);

console.log(JuntarLivros);
```
```js
const administrador = prompt(
  "Seja Bem vindo administrador, por favor insira seu nome para confirmar sua identidade"
);

var Rachide = new Boolean(true);
if (Rachide) {
  console.log("Parabéns! Você se autenticou.");
} else {
  console.log("Você não está autenticado");
}
```
```js
const livros = [
  "javascript Assertivo",
  "Engenharia de Testes",
  "Clean code",
  "Scrum",
  "Guia HTML5 e CSS3",
  "MongoDB"
];

//.includes - retorna um valor booleano, pesquisa se é verdadeiro ou falso.
//.indexof - trás a posição do índice

console.log(livros.indexOf("Amandela"));
//2

console.log(livros.includes("Amandela"));
// true
```
```js
function soma(num1, num2) {
  return num1 + num2;
}

console.log(soma(7, 2));

const compra1 = prompt("Qual o valor da primeira compra?");
const compra2 = prompt("Qual o valor da seguna compra?");

if (compra1 > compra2) {
  console.log(soma(compra1, compra2));
} else if (compra1 < compra2) {
  console.log(subtração(compra1, compra2));
} else {
  console.log("Error");
}

const Mês = prompt("Digite um Mês para saber seu feriado nacional");

switch (Mês) {
  case "Janeiro":
    window.alert("Confraternização Universal");
    break;
  case "Fevereiro":
    window.alert("Carnaval");
    break;
  case "Março":
    window.alert("Paixão de Cristo");
    break;
  case "Abril":
    window.alert("Tiradentes");
    break;
  case "Maio":
    window.alert("Corpus Christi");
    break;
  case "Junho":
    window.alert("São João");
    break;
  case "Julho":
    window.alert("Revolução Constitucionalista");
    break;
  case "Agosto":
    window.alert("Assunção de Nossa Senhora");
    break;
  case "Setembro":
    window.alert("Dia da Independência do Brasil");
    break;
  case "Outubro":
    window.alert("Nossa Senhora Aparecida");
    break;
  case "Novembro":
    window.alert("Consciência Negra");
    break;
  case "Dezembro":
    window.alert("Natal");
    break;
}
```
```js
var PersonagensDeTrigun = ["Vash", "Nicholas", "Meryl", "Mily", "Kuroneko"];
PersonagensDeTrigun.sort();
console.log(PersonagensDeTrigun);

var PersonagensDeTrigun = ["Vash", "Nicholas", "Meryl", "Mily", "Kuroneko"];
var ultimo = PersonagensDeTrigun.pop(); // remove Kuroneko (do final)
// ["Vash", "Nicholas", "Meryl", "Mily"];
console.log(PersonagensDeTrigun);
```

## Atividades desenvolvidas
Trabalho dos vídeos curtos

Atividade Array:

```js
const mangá = ["JJK", "MobPsycho", "OnePiece"];
const Hqs = mangá.concat(["SonicIDW", "Avatar"]);

console.log(mangá); // ["JJK", "MobPsycho", "OnePiece"]
console.log(Hqs); // ["JJK", "MobPsycho", "OnePiece", "SonicIDW", "Avatar"]

const string = Hqs.join("-");

console.log(string); // JJK-MobPsycho-OnePiece-SonicIDW-Avatar

const index = Hqs.indexOf("MobPsycho");

console.log(index); // MobPsycho
```
### Jogo

```js
const movimento = prompt(
  "2 inimigos estão com armas apontadas na sua direção, qual seu proximo movimento? A: Correr em direção aos inimigos com a katana. B: Desviar dos tiros e atacar. C: Tentar defender com a katana."
);

if (movimento == "C") {
  console.log(
    "Você conseguiu defender as 2 balas e finalizou os inimigos, você passou de nível. Proximo nível: https://codepen.io/HueHue-the-animator/pen/KKOKMag "
  );
} else if ("A") {
  console.log("Você avançou e levou 2 tiros dos inimigos, você morreu");
} else if ("B") {
  console.log("Você desviou e lançou sua katana");
  console.log("Você tentou esquivar e levou um dos tiros, você morreu");
}
```
```js
const refém = prompt(
  "Você acha um inimigo e ele está com um refém, oque você faz? A: Você lança a katana na direção deles. B: Parar o tempo e ataca-lo por trás. C: Fazer nada"
);
if (refém == "Parar o tempo e ataca-lo por trás") {
  console.log(
    "Por mais que isso gastou muita energia, você conseguiu eliminar ele sem matar o refém, você passou de nível"
  );
} else if ("Você lança a katana na direção deles") {
  console.log("Você acaba acertando os dois, você falhou");
} else {
  console.log("Você observa ele e ele mata o refém, você falhou");
}
```
