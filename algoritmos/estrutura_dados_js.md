<h1 align="center">Estudo de conceitos basicos em JavaScript</h1>


![image](https://user-images.githubusercontent.com/64383080/157234371-a9cc5eeb-1d00-4710-93a3-f049ab5bdbb3.png)


<p align="center">🚀 Esse estudo visa compreender a logica de programação e conceitos basicos de javascript </p>


<p align="center">
 <a href="#operador">O que é um operador</a> •
 <a href="#igualdade">Operadores de igualdade</a> • 
 <a href="#condicionais">Condicionais</a> • 
 <a href="#lacos">Laços</a> • 
 <a href="#funcoes">Funções</a> • 
 <a href="#poo">Programação Orientada a Objeto</a> • 
 <a href="#fonte">Fonte do estudo</a>
</p>



<h2 align="center" > ➕ ➗ O que é um operador? ➖ ✖️</h2>


<p>Operador são os simbolos que identificam o que sera executado no algoritmo e lógica. Na época de escola conhecemos os operadores aritméticos, eles também são usados na programação mas alguns possuem imagens diferentes. </p>

![image ](https://user-images.githubusercontent.com/64383080/157247063-37d03ccd-d5cd-4889-843b-74a6c80430da.png)

<p>Em programação além das operações aritméticas básicas precisamos em situações comparar uma variável ou condição com outra e nessas situações usamos operadores de comparação 
</p>

![image](https://user-images.githubusercontent.com/64383080/157247327-492ecb72-0f32-462c-abe6-3cb80829e15d.png)


<p>E temos os operadores lógicos, eles servem para ajudar nas função de condicionais como if e for por exemplo.</p>
<p>Um exemplo de uma situação, digamos que você precisa ir ao mercado e comprar arroz, porem para comprar ele tem que seguir alguns requisitos. Esses requisitos podem ser preço <strong>E</strong> validade do produto, ele estando dentro do esperado é para prosseguir com a compra. </p>
<p>Em uma tela de código ficaria:</p>

<p>if( preço===5,00 && validade > 6 meses) {   Seguir com a compra}</p>

![image](https://user-images.githubusercontent.com/64383080/157300566-c4d7eb16-fef1-462d-a084-73fc5a6babcb.png)

<h3 align="center"> Tipos de Saída </h3>

<p>O tipo de saída é a forma como sera nomeado a saída de uma informação. Isso quer dizer que uma informação inserida no sistema sera armazenada com um tipo de dado. Temos dois tipos de dados: 
</p>

<h5>Tipos de dados Primitivos:</h5>

<p>🔸 Null (nulo)</p>
<p>🔸undefined (indefinido)</p>
<p>🔸string (informações textuais geralmente virão entre  “ abc” ou ‘abc’)</p>
<p>🔸number (informações como números)</p>
<p>🔸boolean (booleano conhecidos com condicionais de verdadeiro ou falso)</p>
<p>🔸symbol (simbolos)</p>

<h5>Tipo de dados derivados: </h5>
<p>objetos JavaScript</p>

<br>
<h2 align="center" >Funções e operadores de igualdade (== e ===)</h2>


<p>Os dois operadores de igualdade tem a mesma finalidade de conferir se a extremidade de um lado é igual a outra. Porem os dois tem particularidades para serem usadas em determinado momento. </p>
<p>“Quando == é usado os valores poderão ser considerados iguais mesmo se forem de tipo diferentes. “  Pode parecer meio confuso, mas um exemplo simples você tem uma taça de vinho e um copo de vinho usando == ele ira retornar “true” porque as duas são do mesmo valor “vinho”, porem são de tipos diferentes um é copo e a outra é uma taça.</p>
<p>Ja === é uma validação que ira avaliar se o tipo e o valor são iguais não apenas um dos itens, mas ele todo. Caso seja diferente retornará “false”.</p>


<h2 align="center" >Instruções de condicionais</h2>

<p>Primeiramente, o if serve para analise de uma condição, como no exemplo do supermercado.
A primeira instrução de condicional que analisaremos é a construção if...else. Há algumas maneiras de usar essa construção. 
</p>
Podemos fazer um if para retornar um valor positivo tipo:

if (numero === 1) {
	console.log(‘numero é igual a 1’
} 

<p>Ou podemos retornar um if com eles, que resumindo se uma condição for verdadeira fazer x condição, se ela for falsa fazer outra condição.</p>

![image](https://user-images.githubusercontent.com/64383080/157304466-e2545901-e997-4150-8452-dbf6cd1a20d3.png)

<p>Outra forma de fazer uma condicional que contém várias condições é através do else if, o que seria? continuar a codificação até a conclusão de todas as validações.
exemplo
</p>


![image](https://user-images.githubusercontent.com/64383080/157304538-c409225d-93ba-4f8a-a045-1b1a4506dd4c.png)

<h5>
Temos também o switch
</h5>
“Se a condição que estivermos avaliando for a mesma que a anterior (porém a comparação é feita com valores diferentes) podemos usar a instrução switch

![image](https://user-images.githubusercontent.com/64383080/157304844-3679d142-afd5-45d7-a186-1853cb2c0fbd.png)

<h2 align="center" >Laços</h2>

<p></p>

<p>Laços são usados com frequência quando trabalhamos com arrays. Ele é constituído de um contador e ira seguir uma repetição ate o fim da condição.
Exemplo: for
</p>

![image](https://user-images.githubusercontent.com/64383080/157305143-22ad35a5-6055-40e7-9619-88fa6ff7d8de.png)


<p>Outro laço conhecido é o while o bloco de código dentro do laço while será executado enquanto a condição for verdadeira. </p>

![image](https://user-images.githubusercontent.com/64383080/157305294-c4c8c8c6-1190-4b64-9608-3a61806487b0.png)


<h2 align="center" >Funções</h2>

<p>As funções são muito importantes em JavaScript, e tera muito uso de função no js.
O código a seguir mostra a sintaxe básica de um função
</p>

![image](https://user-images.githubusercontent.com/64383080/157305568-d3ec2ef3-db9e-49e9-a87b-e1e8cea0d362.png)


<p>Para que usamos função no código?</p>

<p>Segundo 
“A ideia básica de uma função, implementada em alguma linguagem de programação, é encapsular um código que poderá ser invocado/chamado por qualquer outro trecho do programa. Seu significado e uso são muito parecidos com o de funções matemáticas, ou seja, existe um nome, uma definição e posterior invocação à função.” Leonidas brandão link. Fonte:
</p>

<a> <https://www.ime.usp.br/~leo/mac2166/2017-1/introducao_funcoes.html></a>

<h2 align="center" >Programação Orientada a Objetos "POO"</h2>

<p></p>

<p>“Um objeto é uma instância de classe. Uma classe define as caracteristicas de um objeto” LoianeGroner </p>

![image](https://user-images.githubusercontent.com/64383080/157306330-c043eb53-b86b-426d-a35e-ac003820d25e.png)

![image](https://user-images.githubusercontent.com/64383080/157306651-074c4ec3-fb1a-4c70-9093-97bf6947235a.png)

Para entender melhor segue um link de uma fonte do youtube para complementar o entendimento
<a>https://www.youtube.com/watch?v=_RKKKDlqi2Q</a>

<h2 align="center" > 🛠 fonte </h2>

As seguintes anotações tiveram como base:

### 📚 Estrutura de Dados e Algoritmo com JavaScript - Loiane Groner
### 📄  Documentação javascript:

<a>https://developer.mozilla.org/pt-BR/docs/Web/JavaScript</a>

### 💻 youtube.com.br