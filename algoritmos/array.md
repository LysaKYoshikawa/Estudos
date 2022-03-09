<h1 align="center">Arrays</h1>

![image](https://user-images.githubusercontent.com/64383080/157354030-26ca094f-c502-4c81-aec0-b982f5ea35d2.png)



<p align="center">🚀 Estudo para entender array e sua logica </p>

<p align="center">
 <a href="#operador">O que é ECMAScript</a> •
 <a href="#igualdade">arrow functions</a> • 
 <a href="#condicionais">POO</a> • 
 <a href="#lacos">Herança</a> • 
 <a href="#funcoes">Getters e Setters</a> • 
 <a href="#poo">TypeScript</a> • 
 <a href="#fonte">Fonte do estudo</a>
</p>


<h2 align="center"> O que é uma Array? </h2>
Um array é uma estrutura de dados. Em todas as linguagens de programação possuem um tipo de dado array incluído. Um array armazena valores que são todos do mesmo tipo.

### Por que usar Array?

Imagina que você precisa armazenar as temperaturas medias de uma cidade, bem poderia ser feito isso declarando variaveis com as temperaturas medias de cada mês, porem supondo que agora fosse necessario armazenar de varios anos, fica inviável armazenar em varias variáveis a mesma informação.

Para isso foi criado o array, uma estrutura de dados que ira armazenar valores do mesmo tipo, sendo assim ao invés de ter 

![image](https://user-images.githubusercontent.com/64383080/157355658-499f4207-0614-49f5-9370-87b264390f06.png)

pode ter: 

![image](https://user-images.githubusercontent.com/64383080/157355678-98677c6d-3b44-4449-b888-df373e9ba293.png)

Em javaScript, um array é um objeto mutável. Podemos facilmente lhe acrescentar ou tirar elementos. Em outras linguagens como java, por exemplo, precisa indicar o tamanho do array e caso precise acrescentar novos elementos um novo array precisará ser feito.

<h2 align="center"> Acrescentando Elementos </h2>

![image](https://user-images.githubusercontent.com/64383080/157356319-4e50d4ce-b35e-4cb2-9277-54a8e2281a25.png)

<h2 align="center">Removendo Elementos  </h2>
usando pop() e shift()

![image](https://user-images.githubusercontent.com/64383080/157356416-6d4e63eb-f4bd-4b1e-85fb-417f77f4e8e7.png)

<h2 align="center"> Adicionando ou removendo elementos de uma posição especifica.</h2>

É possível remover ou adicionar elementos em uma posição específica. Para remover de uma posição específica podemos usar slice indicando a posição.

![image](https://user-images.githubusercontent.com/64383080/157357043-fdb497a6-417f-42a9-95a5-4d01bf9981ee.png)

E para acrescentar de uma posição especifica podemos tambem usar o splice indicando a posição, o numero que deseja tirar ou não, e o aa quantidade para acrescentar

exemplo numbers.splice(5, 0, 5,6,7)


- 5 equivale a posição do array
- 0 equivale que não deseja remover nenhum elemento
- 5,6,7 equivale aos numero que deseja incluir no array

![image](https://user-images.githubusercontent.com/64383080/157357191-ef851d5a-f020-42c8-a7c4-b02f44a19458.png)


<h2 align="center">Arrays Bidimensionais e Multidimensionais</h2>

Um array bidimensional é uma matriz também conhecida como array de arrays. No exemplo dado sobre temperaturas do início do capitulo, era criando um array simples armazenado as temperaturas medias, porem imagine que agora a necessidade é guardar as informações de temperatura de uma cidade por hora. 

O que seria um array de arrays, seria um array em que cada elemento puxa outra array
seguindo exemplo do livro 

![image](https://user-images.githubusercontent.com/64383080/157357324-d2238a2c-fe5f-4695-a6c8-edf50209261c.png)

Outra forma de declarar arrays assim 

![image](https://user-images.githubusercontent.com/64383080/157357537-b0b28967-2c34-4d54-b329-a31cc2947e4c.png)

onde temos o dia como [0] [1] e as horas na frente [1] [2] [3]... e os números que seriam as temperaturas.

![image](https://user-images.githubusercontent.com/64383080/157357632-1cd6adde-da98-4fa6-8167-35805a4cc813.png)

<h2 align="center">Referências aos métodos arrays em javaScript</h2>

Tem alguns mais metodos paa serem usados em arrays que pode simplificar o codigo e seu entendimento.

concat

every

filter

forEach

join

indexOf

lastIndexOf

map

reverse

slice

some 

sort 

toString

valueOf

### Juntando Arrays
Supondo um cenário que temos varios arrays e queremos juntar eles. Uma forma de fazer isso seria através do concat passando por dentro dele os arrays que deseja juntar.

### Interação com Every
Ele itera todos os elementos do array verificando se a condição desejada (função) ate que false seja devolvido. Seria como um &&

### Interação com some
Parecido com o every porem ele faz a interação com o array, verificando a condição desejada, ate que true seja devolvido. Seria como um || 

### Interação com foreach
Se precisar fazer a iteração em todo array independente de tudo podemos usar um forEach o resultado sera o mesmo que um laço for.

### Usando map
O Map ele devolve um array a partir de uma função que contem um critério ou condição e devolve elementos do array que correspondam aos critérios.

### Usando Filter
Ele devolve um array porem os elementos filtrados, que foi passado pela condição ou função

### Usando o método reduce
Por fim temos o método reduce recebe uma função com o mesmo nome com os seguintes parâmetros: 

Acumulador (acc)
Valor Atual (cur)
Index Atual (idx)
Array original (src)

podemos usar esse método para devolver um valor que sera somado a um acumulador, o qual será devolvido depois que o método reduce parar de executar

![image](https://user-images.githubusercontent.com/64383080/157358099-2008ea5a-1ed3-47f4-b442-a8c8b2b03c1c.png)


<h2 align="center">Novas funcionalidades com Array </h2>
nas novas atualizações do ES2016 foi apresentado novas funcionalidades aos arrays 

![image](https://user-images.githubusercontent.com/64383080/157358694-e20498cb-60eb-43ae-a8d9-f4f3018f12cf.png)


<h2 align="center"> Método entries, keys e values </h2>

Resumindo seria uma interação de chave e valor, em outras palavras o método entries desenvolve um iterador que contem chave e valor 

Lembrando do array numbers 

![image](https://user-images.githubusercontent.com/64383080/157358778-8ab62aa0-c263-432a-9781-64b109f1a0aa.png)

<h2 align="center" > 🛠 fonte </h2>

As seguintes anotações tiveram como base:

### 📚 Estrutura de Dados e Algoritmo com JavaScript - Loiane Groner
### 📄  Documentação javascript:

<a>https://developer.mozilla.org/pt-BR/docs/Web/JavaScript</a>

### 💻 <a>https://www.youtube.com/results?search_query=stack+com+js</a>

### 💻 <a>https://www.udemy.com/course/curso-web/learn/lecture/9129740?start=105#overview</a>
