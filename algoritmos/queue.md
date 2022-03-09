<h1 align="center">Queue / Fila</h1>

![image](https://user-images.githubusercontent.com/64383080/157361673-0109f798-a393-4c2c-abba-b7b0d32ad0ea.png)



<p align="center">🚀 Estudo de estrutura de dados com pilhas </p>

<p align="center">
 <a href="#operador">O que é uma fila?  </a> •
 <a href="#igualdade">Métodos disponíveis em uma fila</a> • 
 <a href="#condicionais">Criando o metodo ToString </a> • 
 <a href="#lacos">Usando a classe Queue</a> • 
 <a href="#funcoes">Usando uma classe Queue</a> • 
 <a href="#funcoes">Estrutura de dados Deque</a> • 
 <a href="#funcoes">Metodos da classe Deque </a> • 
 <a href="#funcoes">Usando classe Deque</a> • 
 <a href="#funcoes">Usando uma classe Queue</a> •
 
  <h2 align="center">O que é uma fila?</h2>
  Fila em ingles Queue é uma coleção ordenada baseada na FIFO (Frist in Frist Out, isto é o primeiro que entra é o primeiro que sai) a adição de elemento ocorre em cauda e a remoção é na frente ou seja o primeiro elemento que entrou.

Um exemplo na vida real poderia ser uma fila de supermercado o primeiro que entrou, aquele que esta mais proximo do caixa, sera primeiro atendido que o ultimo que entrou na fila.

  <h2 align="center">Métodos disponíveis em uma fila </h2>

  - enqueue(element): esse método adiciona um novo elemento no final da fila

- dequeue(): esse método remove o primeiro elemento no final da fila. Também devolve o elemento que saiu da fila
- peek(): esse método devolve o primeiro elemento da fila. Funciona como o método front como é conhecimento em outras linguagens 
- isEmpty(): esse método devolve true se a fila não contiver nenhum elemento e false se o tamanho for maior que 0.
- size(): esse método devolve o numero de elementos contidos na fila. É semelhante à propriedade length do array.

  <h2 align="center">Criando o metodo ToString</h2>

  Assim como no stack no queue tambem podemos acrescentar um toString 

  ![image](https://user-images.githubusercontent.com/64383080/157431627-e048f379-8e0c-4e16-820a-b802bfb99ba5.png)

  As classes Queue e Stack são muito parecidas. A única diferença esta nos métodos dequeue e peek, que se deve à distinção entre os princípios FIFO e LIFO.


  <h2 align="center">Usando a classe Queue</h2>
  Inicialmente devemos instanciar a classe que criamos 

  ![image](https://user-images.githubusercontent.com/64383080/157431684-00dfa8bd-477b-41b6-be2c-c5a13e662f9a.png)

  no exemplo acima mostra uma fila vazia e depois a inclusão de dois nomes. Como trata-se de uma fila, o primeiro que entrou foi Maju e depois Raphaela.

Acrescentei mais um elemento a fila ficou assim:

![image](https://user-images.githubusercontent.com/64383080/157431711-8c80305b-1d8e-4e05-9c8c-1b8e54e92716.png)

com o metodo empty verifica se esta vazia.

A lógica abaixo mostra a execução de uma classe queue

![image](https://user-images.githubusercontent.com/64383080/157431994-17f0e5d4-2039-4cc1-a227-b18c2cfe7b3c.png)


  <h2 align="center">Usando uma classe Queue</h2>

  A estrutura de dados deque tambem conhecida como fila de duas pontas (double-ended queue), é uma fila especial que nos permite inserir e remover elementos do final ou da frente da fila.
Um exemplo do cotidiano seria uma fila de lanchonete que o ultimo membro da fila pode ser atendido por ser idoso, assim como o primeiro membro da fila.

<h1 align="center">Estrutura de dados Deque</h1>

A estrutura de dados deque também é conhecida como fila de duas pontas (double-ended queue), é uma fila especial que nos permite inserir e remover elementos do final ou da frente da fila.

Um exemplo do cotidiano seria uma fila de lanchonete que o ultimo membro da fila pode ser atendido por ser idoso, assim como o primeiro membro da fila.



  <h2 align="center">Metodos da classe Deque</h2>

  - addFront(element) : esse metodo adiciona um elemento na frente do deque
- addBack(element): esse metodo adiciona um elemento no fim do deque
- removeFront(): ele remove o primeiro elemento do deque
- removeBack(): esse metodo remove o ultimo elemento do deque
- peekFront(): edde devolve o primeiro elemento do deque.
- peekBack(): esse devolver o ultimo elemento do deque.

a classe deque tambem implementaos metodos isEmpty, clear, size e toString.

  <h2 align="center">Usando classe Deque</h2>
  Aqui embaixo fiz um teste de uso de deque

![image](https://user-images.githubusercontent.com/64383080/157432349-f55027bc-a3eb-4fac-83ca-e093754ccc76.png)

<h2 align="center" > 🛠 fonte </h2>

As seguintes anotações tiveram como base:

### 📚 Estrutura de Dados e Algoritmo com JavaScript - Loiane Groner
### 📄  Documentação javascript:

<a>https://developer.mozilla.org/pt-BR/docs/Web/JavaScript</a>

### 💻 <a>https://www.youtube.com/results?search_query=stack+com+js</a>

### 💻 <a>https://www.udemy.com/course/curso-web/learn/lecture/9129740?start=105#overview</a>
