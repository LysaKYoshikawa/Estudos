<h1 align="center">Conceitos de ecmascript</h1>


<p align="center">🚀 Esse estudo visa compreender Os conceitos de EcmaScript assim como conceitos de atualizações  </p>

<p align="center">
 <a href="#operador">O que é ECMAScript</a> •
 <a href="#igualdade">arrow functions</a> • 
 <a href="#condicionais">POO</a> • 
 <a href="#lacos">Herança</a> • 
 <a href="#funcoes">Getters e Setters</a> • 
 <a href="#poo">TypeScript</a> • 
 <a href="#fonte">Fonte do estudo</a>
</p>


<h2 align="center">O que é ECMAScript </h2>

O que é ECMAScript é uma organização que padroniza informações. E a muito tempo atrás JavaScript foi submetido a ECMA para que fosse padronizada. O que resultou em um novo padrão de linguagem.

### Curiosidade
As versão ES2016 é a mesma coisa que (ES7), o motivo de seguir essa ordem é que qdo foi lançado em junho de 2015, ECMA2015 (ES2015) quase 6 anos depois da última versão o nome (ES6) se tornou popular antes do lançamento do ES2015.

<h3>O LET</h3>
O let entra no lugar do var e é uma forma de declarar as variáveis do código porém elas não podem mudar de valor no mesmo escopo ex:
let fruta = 'banana';
let fruta = 'goiaba' // vai apresentar um erro

Pq está no mesmo ambiente de escopo

Porém

let fruta = 'banana' ;

function quintanda() {
fruta = 'chuchu';
return fruta;
}

console.log(fruta) //vai retornar 'chuchu'
Ou seja let pode ser alterado fora do escopo.

<h3>O Const</h3>
Const será o valor declarado que será para leitura e de valor constante ou seja não terá mudanças. Const não aceita mudanças. Por ela ser uma variavel local, sendo assim ela só sera executada dentro do codigo.

![image](https://user-images.githubusercontent.com/64383080/157348748-a9e1b0b8-b2cf-4601-8449-cff3fe5d88c3.png)

Na forma a seguir ele funciona melhor:

![image](https://user-images.githubusercontent.com/64383080/157348837-0935ae78-5ee8-4d29-a5fd-1890c5e94656.png)


<h3>Templates literais</h3>

É uma forma criar strings sem a necessidade de concatenar valores

![image](https://user-images.githubusercontent.com/64383080/157348946-246e0df3-5fe0-425f-8372-7d2cfb152230.png)


<h2 align="center">Funções de Seta (arrow functions)
 </h2>

 ### As funções de seta é uma forma de simplificar o a sintaxe das funções. De inicio pode parecer estranho, mas com pratica percebera que é muito facil e ate em alguns casos mais simples de escrever e entender o código.

![image](https://user-images.githubusercontent.com/64383080/157349981-700163a6-aa20-4ac2-9924-e3b621e014cb.png)

Se a função ainda tiver uma unica instrução, podemos usar uma versao mais simples omitindo a palavra reservada return e as chaves:
![image](https://user-images.githubusercontent.com/64383080/157350051-223efc5b-0036-42ac-87b3-062d6f2b5cdc.png)
resultado : 

![image](https://user-images.githubusercontent.com/64383080/157350112-ec5aeddc-c159-4473-9a56-ea280b3d8c6a.png)


<h2 align="center"> Programação Orientada a Objeto
</h2>
Na ES2015 tambem lançou uma maneira mais simples de declarar classes 

![image](https://user-images.githubusercontent.com/64383080/157350722-1f8c9074-ff98-47d6-93a5-ac1dd6859855.png)

Da para declarar uma classe como no exemplo de class Book com uma função construtor alem de outras como no exemplo do printIsbn().

<h2 align="center"> Herança</h2>

<strong> Herança </strong> refere-se a habilidade de um objeto acessar métodos e outras propriedades de outro objeto.
Podemos fazer isso inserindo extends e estender outra classe e herdar seu comportamento. Pode-se tambem referenciar o construtor usado na outra classe usando a palavra reservada <strong> super </strong>

![image](https://user-images.githubusercontent.com/64383080/157351102-609f48f6-f11d-430f-a145-1a300110b037.png)


<h2 align="center">Getters e Setters</h2>

Na atualização ES2015 é possível declarar uma função com get e/ou set. Mesmo os atributos de classe não sendo privados, mas é bom utilizar um padrão. Para declarar uma função get e set, basta usar a palavra reservada get ou set na frente da função, o nome que queremos expor será usado.

<h3>Modulos</h3>

Os modulos são um codigojs declarado em arquivos separados. Podemos importar as funções, as variáveis e as classes de outros arquivos diretamente no código javascript. Com os modulos podemos organizar melhor o código principalmente em um projeto grande.

![image](https://user-images.githubusercontent.com/64383080/157352304-a6122388-ef65-4083-b87c-a45f901c4bd0.png)

Podemos também adicionar a palavra export no inicio de cada função ou variável assim não sera necessario inserir o export no final do arquivo

![image](https://user-images.githubusercontent.com/64383080/157352382-280f6cba-5b9f-41bd-af73-e3bdfd908a75.png)

pode também renomear as funções quando elas forem exportadas

![image](https://user-images.githubusercontent.com/64383080/157352622-f95b9de5-9b53-4581-9c96-acbcd5dbed5b.png)

<h2 align="center"> TypeScript </h2>

O typeScript é um superconjunto  gradualmente tipado de javascript, com o codigo aberto, criado e mantido pela Microsoft. Ele foi criado para desenvolvedores pudessem potencializar a linguagem javascript 

<h3>Interface</h3>
Interface funciona como um contrato entre si e qualquer classe ou estrutura que implemente sua interface.
Em Typescript exitem dois conceitos de interfaces.
No primeiro esta relacionado a atribuição de um tipo a uma variavel ex:

![image](https://user-images.githubusercontent.com/64383080/157352965-9c3c0c88-bf5b-46c4-9ccc-c3055cddbc13.png)

nesse conceito ele permite que tenha um preenchimento automático

O segundo conceito de interface em typescript esta relacionado a orientação a objeto como é feito em outras linguagens como java, c#, Ruby e assim por diante. no exemplo abaixo mostra como aplicar o segundo conceito de interface em typeScript

![image](https://user-images.githubusercontent.com/64383080/157353222-1968fb6c-c0a7-45d2-ae27-baf2c9f2bd8f.png)

<h2 align="center">Fonte do estudo </h2>
As seguintes anotações tiveram como base:

### 📚 Estrutura de Dados e Algoritmo com JavaScript - Loiane Groner
### 📄  Documentação javascript:

<a>https://developer.mozilla.org/pt-BR/docs/Web/JavaScript</a>

### 💻 youtube.com.br
