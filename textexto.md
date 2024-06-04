##Introdução
JavaScript é uma das linguagens de programação mais populares, amplamente utilizada para desenvolvimento web. Este artigo apresenta algumas das funções mais importantes e úteis do JavaScript, com exemplos práticos para ajudá-lo a entender seu uso em contextos reais.

##Funções de Manipulação de Arrays

###map()
A função map() cria um novo array com os resultados de chamar uma função para cada elemento do array.

const numeros = [1, 2, 3, 4];
const dobrados = numeros.map(num => num * 2);
console.log(dobrados); // [2, 4, 6, 8]

###filter()
A função filter() cria um novo array com todos os elementos que passaram no teste implementado pela função fornecida.

const idades = [15, 18, 21, 17, 30];
const adultos = idades.filter(idade => idade >= 18);
console.log(adultos); // [18, 21, 30]

###reduce()
A função reduce() aplica uma função a um acumulador e a cada valor do array (da esquerda para a direita) para reduzi-lo a um único valor.

const valores = [1, 2, 3, 4];
const soma = valores.reduce((acumulador, valorAtual) => acumulador + valorAtual, 0);
console.log(soma); // 10

##Funções de Manipulação de Strings

###toUpperCase()
A função toUpperCase() converte uma string para letras maiúsculas.

const saudacao = "olá, mundo!";
const saudacaoMaiuscula = saudacao.toUpperCase();
console.log(saudacaoMaiuscula); // "OLÁ, MUNDO!"

###includes()
A função includes() verifica se uma string contém uma determinada substring.

const frase = "JavaScript é incrível";
const temJavaScript = frase.includes("JavaScript");
console.log(temJavaScript); // true

##Funções de Manipulação de Objetos

###Object.keys()
A função Object.keys() retorna um array contendo as chaves de um objeto.

const pessoa = { nome: "Ana", idade: 25, cidade: "São Paulo" };
const chaves = Object.keys(pessoa);
console.log(chaves); // ["nome", "idade", "cidade"]

###Object.values()
A função Object.values() retorna um array contendo os valores das propriedades de um objeto.

const pessoa = { nome: "Ana", idade: 25, cidade: "São Paulo" };
const valores = Object.values(pessoa);
console.log(valores); // ["Ana", 25, "São Paulo"]

###Object.entries()
A função Object.entries() retorna um array de pares [chave, valor] do objeto.

const pessoa = { nome: "Ana", idade: 25, cidade: "São Paulo" };
const entradas = Object.entries(pessoa);
console.log(entradas); // [["nome", "Ana"], ["idade", 25], ["cidade", "São Paulo"]]

##Funções Assíncronas

###async e await
As palavras-chave async e await são usadas para lidar com operações assíncronas de forma mais legível.

async function fetchData() {
  try {
    const response = await fetch('https://api.exemplo.com/dados');
    const dados = await response.json();
    console.log(dados);
  } catch (erro) {
    console.error('Erro ao buscar dados:', erro);
  }
}

fetchData();

##Funções Anônimas e Arrow Functions

###Funções Anônimas
Funções anônimas são funções sem nome que são frequentemente usadas como argumentos para outras funções.

setTimeout(function() {
  console.log('Executado após 2 segundos');
}, 2000);

##Arrow Functions
Arrow functions são uma forma mais concisa de escrever funções em JavaScript. Elas são especialmente úteis para funções anônimas.

setTimeout(() => {
  console.log('Executado após 2 segundos');
}, 2000);

const numeros = [1, 2, 3, 4];
const dobrados = numeros.map(num => num * 2);
console.log(dobrados); // [2, 4, 6, 8]


##Manipulação de Datas

###Date()
A função Date() é usada para criar um novo objeto de data.

const hoje = new Date();
console.log(hoje); // ex: Fri Jun 04 2024 10:15:30 GMT-0300 (Brasilia Standard Time)

###getFullYear()
A função getFullYear() retorna o ano de uma data.

const hoje = new Date();
const ano = hoje.getFullYear();
console.log(ano); // 2024

##Conclusão
Estas são apenas algumas das muitas funções úteis disponíveis em JavaScript. Ao dominar essas funções, você estará bem equipado para manipular arrays, strings, objetos, datas e lidar com operações assíncronas de maneira eficiente em seus projetos. Pratique usando esses exemplos em seus próprios códigos e veja como eles podem simplificar seu trabalho de programação!

Features

Usamos neste projetos prompts no chatGPT
Imagens do acervo Lexica.ai

Gostou do conteúdo? Aprenda ainda mais!

Esse conteudo foi gerado por uma inteligencia artificial e foi revisado por um humano eu aqui kkk se conecti comigo no meu linkdin

Vamos juntos nesse Jornada!!! 🚀

