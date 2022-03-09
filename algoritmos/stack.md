<h1 align="center">Pilhas</h1>


<p align="center">🚀 Estudo de estrutura de dados com pilhas </p>

<p align="center">
 <a href="#operador">O que é uma pilha? </a> •
 <a href="#igualdade">Métodos para Stack</a> • 
 <a href="#condicionais">Stack baseada em objeto </a> • 
 <a href="#lacos">Método toString para objeto js</a> • 
 <a href="#funcoes">Classes WeakMap - modo private</a> • 
 
</p>

<h2 align="center">O que é uma pilha?</h2>
É uma coleção ordenada de itens que obedece ao principio LIFO (Last In Frist Out, ultimo a entrar é o primeiro a sair). Por exemplo uma pilha de livros é um exemplo da estrutura de dados pilhas. O histórico de um computador por exemplo também pode ser considerado uma pilha, se der aquela seta para voltar a página anterior ele ira para a última página que visitou saindo da atual que se encontra e fazendo da última página que visitou a primeira que iniciou a busca.

<h2 align="center">Métodos para Stack</h2>

- push(element(s)): Esse métodos adiciona um novo elemento (ou varios elementos) no topo da pilha

- pop(): esse método remove o elemento que esta no topo da pilha. Também devolve o elemento removido
- peek(): esse método devolve o elemento que esta no topo da pilha. A pilha não é modificada (o elemento não é removido; ele é devolvido apenas como informação)
- isEmpty(): esse método devolve true se a pilha não contiver nenhum elemento e false se o tamanho da pilha for maior que 0.
- clear(): esse método remove todos os elementos da pilha.
- size(): esse método devolve o número de elementos contidos na pilha. É semelhante à  propriedade length de um array.

### Push de elementos na pilha 
O Push de novos elementos em uma pilha comum tem  apenas um detalhe importante é que ao adicionar os novos itens iram para o topo da pilha, isto é o final da pilha.

![image](https://user-images.githubusercontent.com/64383080/157360251-d96a61dd-cf57-4ae7-883a-0217420cfd82.png)

### Pop de elementos da pilha

Com pop pode ser removido um elemento da pilha, porem como a pilha segue o principio de LIFO, onde o ultimo elemento que entrou é o primeiro a sair, então na hora de remover elementos o ultimo elemento que entrou será o que vai sair.

### Método peek

Se quiser olhar, por exemplo o ultimo elemento adicionado na pilha podera usar o método peek().

peek(){
	return this.items[this.items.length - 1];
}

Como internamente esta um array para analise então coloca-se o -1 para saber o ultimo elemento com o length. Ou seja se a pilha tiver 3 números 

topo
2 - 400
1 - 52
0 - 23 - base

internamente o calculo ira pegar 3 posições - 1 e o resultado sera o índice 2 valor 400

### Metodo isEmpty

Esse devolvera true se a pilha estiver vaziae false se o contrario


isEmpty(){
	return this.items.length === 0;
}

verificar se o tamanho interno é igual a 0.

<h2 align="center">Stack baseada em objeto</h2>

Ao criar um classe Stack ela é usa um array para armazenar elementos. Ao trabalhar com um conjunto grande e dados, também sera necessario analisar qual o modelo mais eficaz de manipular os dados. Se for um array de muitos elementos o código ira demorar mais interar por eles.Nessas situações é possivel usar objeto js para armazenamentos da pilha, mantê los em ordem e obedecer igualmente ao principio LIFO.

<h2 align="center">Método toString para objeto js</h2>

Na versão de código com objeto dá para criar um método toString para que possamos exibir o conteúdo da pilha de modo semelhante a um array.

<h2 align="center">Classes WeakMap - modo private</h2>

Uma forma de private da sua pilha para promover segurança e, adcionar ou remover ou renomear suas pilhas é usando WeakMap. 

“Precisamos saber que um WeakMap é capaz de armazenar um par chave/valor, no qual a chave é um objeto e o valor pode ser um dado de qualquer tipo.” page 122

<h2 align="center" > 🛠 fonte </h2>

As seguintes anotações tiveram como base:

### 📚 Estrutura de Dados e Algoritmo com JavaScript - Loiane Groner
### 📄  Documentação javascript:

<a>https://developer.mozilla.org/pt-BR/docs/Web/JavaScript</a>

### 💻 <a>https://www.youtube.com/results?search_query=stack+com+js</a>

### 💻 <a>https://www.udemy.com/course/curso-web/learn/lecture/9129740?start=105#overview</a>