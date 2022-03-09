<h1 align="center">Listas Ligadas em Js</h1>

![image](https://user-images.githubusercontent.com/64383080/157435137-e886131d-2933-4f65-9b9e-51d49bdd6be3.png)




<p align="center">🚀 Estudo para entender conceitos de Listas Ligadas e suas variações </p>

<p align="center">
 <a href="#operador">Listas ligadas</a> •
 <a href="#igualdade">Métodos da LinkedList</a> • 
 <a href="#condicionais">Conceito de listas duplamente ligada</a> • 
 <a href="#lacos">Listas Ligadas circulares </a> • 
 <a href="#funcoes">Listas Ligadas Ordenadas</a> • 
 <a href="#poo">Classe StackLinkedList</a> • 
 <a href="#fonte">Fonte do estudo</a>
</p>

<h2 align="center"> </h2>
<h1 align="center"></h1>

<h1 align="center">Listas Ligadas</h1>
Lista ligada é uma estrutura de dados dinâmica.

Na maioria das outras linguagens de programação uma array é de tamanho fixo ou seja não é tão simples inserir ou retirar elementos podendo ser até custoso devido o deslocamento dos elementos. Em Javascript já vimos que temos métodos que farão isso para nós, porém também tem um deslocamento de elemento e isso também é custoso. 

As listas ligadas armazenam uma coleção sequencial de elementos, porém diferentemente do array os elementos não são posicionados de forma contínua na memória. Cada elemento da lista é constituído de um nó e uma referencia que aponta para o proprio elemento conhecido como ponteiro.

A principal característica de uma lista ligada é que não é necessário deslocar elementos quando um novo elemento é adicionado ou removido, como cada elemento é um nó basta retirar o elemento, entretanto devido ao seu ponteiro que mostra o elemento proximo tem que tomar uma atenção especial.

Um exemplo de lista ligada na vida real, seria um trem cada vagão é um elemento e as ligações entre os vagos seriam o ponteiro 

![image](https://user-images.githubusercontent.com/64383080/157437780-f3237977-af85-429d-bb41-194a93415e7a.png)



<h2 align="center">Métodos da LinkedList </h2>

- push(element):Esse método adiciona um novo elemento no final da lista
- insert(element, position): esse método insere um novo elemento
- getElementAt(index): esse método devolve o elemento que está em uma posição específica  da lista
- remove(element): este método remove um elemento da lista
- indexof(element): esse método devolve o índice do elemento na lista. Se o elemento não estiver na lista, -1 será devolvido
- removeAt(position): esse método remove um item de uma posição específica da lista

<h1 align="center">Lista Duplamente Ligada</h1>

A principal diferença entre a lista duplamente ligada e a lista ligada é que a lista duplamente ligada fazemos uma ligação para o proximo elemento e outra para o elemento anterior

exemplo

![image](https://user-images.githubusercontent.com/64383080/157437993-3b1c9b56-591b-43f1-b4a6-394c12bfe024.png)

Em uma lista ligada simples quando passamos quando inteiramos e passamos do elemento desejado, é necessario retornar ao inicio da lista e reiniciar a iteração. Essa é uma das vantagens da lista duplamente ligada porque pode ir para frente e para tras de um elemento mesmo que passe por ele.

<h1 align="center">Listas Ligadas circulares </h1>

Uma lista ligada circular está relacionada à direção da referência. Como assim? Uma lista ligada simples tem uma ligação com o próximo elemento através de um ponteiro, uma lista duplamente ligada tem uma ligação tanto com o próximo elemento como um anterior e uma lista ligada circular quando interage pela lista e chegar ao último elemento, ele não fará referência a uma elemento <strong> undefined </strong> mas sim para o primeiro elemento.


Como mostra na imagem abaixo 

![image](https://user-images.githubusercontent.com/64383080/157438256-0e93c1c6-86cb-4cb0-8768-4a0db1dfe8c5.png)

<h1 align="center">Listas Ligadas Ordenadas</h1>
A lista ligada Ordenada é uma lista que trará uma  ordem aos elementos ordenados.
Para manter uma lista ordenada, em vez de aplicar um algoritmo de ordenação, inserimos element em sua posição correta  a fim de manter a lista  sempre ordenada.

A classe SortedLinkedList herdara todas as propriedades e os métodos da classe LinkedList, mas como essa classe tem um comportamento especial, precisamos de uma função para comparar elementos.

Inserir elementos nessa lista também precisará ser ordenado.


<h1 align="center">Classe StackLinkedList</h1>

Também podemos usar a classe LinkedList e suas variantes como estrutura de dados internos a fim de criar outras estrutura de dados  como pilha, fila e deque. 

Na classe StackLinkedList, em vez de usar um array ou um objeto JS para armazenar itens é usado uma DoublyLinkedList no caso de pilha,a inserção será no final da pilha e a sua retirada também.

<h2 align="center" > 🛠 fonte </h2>

As seguintes anotações tiveram como base:

### 📚 Estrutura de Dados e Algoritmo com JavaScript - Loiane Groner
### 📄  Documentação javascript:

<a>https://developer.mozilla.org/pt-BR/docs/Web/JavaScript</a>

### 💻 <a>https://www.youtube.com/results?search_query=Lista+ordenadas+com+js</a>

### 💻 <a>https://www.udemy.com/course/curso-web/learn/lecture/9129740?start=105#overview</a>