<h1 align="center"> 📘 Capítulo Comentários</h1>

Conceitos e entendimentos do livro Clean Code - Resumo dissertativo 
Esse capitulo o autor trouxe pontos de vistas em relação a comentários em código.

indice 
<p align="center">
 <a href="#">Por que não comentar</a> •
 <a href="#">Quando comentar?</a> • 
 <a href="#">Comentários ruim?</a> • 

</p>


<h2 align="center"> 🔹 Por que não comentar?</h2>

Segundo o entendimento e o que o autor trouxe, ele não indica fazer comentarios em códigos. Muitas vezes refatorar o código ou função é melhor que exercer um comentário.

No livro ele traz que comentários são ruim porque muitas vezes o que foi colocado como comentário não condiz com o que a função ou trcho de código faz.

Em certas ocasioes o comentário pode estar desatualizado com a finalidade da função

O comentário tambem pode estar atrapalhando o entendimento da função, pelo costume temos a mania de ler o código e depois o comentário e isso pode atrapalhar o entendimento.

<h2 align="center"> 🔹 Quando comentar?</h2>

O autor explica que tem situações que o comentário é necessário, mas são momento muito posuais.

Em situações que o comentário esta trazendo direitos autorais ou informações necessarias do funcionamento é um momento de um comentário breve e direto.

Comentarios informativos, são comentário informando o que uuma função ou trecho de código esta retornando, porem o autor disse tambem que nesse casos vale reavaliar os nomes porque as vezes renomeando o nome da função ou variável ficará fácil de entender e sem precisar de comentário.

Comentários de esclarecimento, quando você traz um comentário esclarecendo o que o parâmetro ou valores estão retornando. 

Comentário de alerta de consequencias, as vezes é necessário um comentário avisando uma consequência do código. No exemplo do livro:

```
//Não execute a menos que você tem tempo disponível.
```

Comentários To Do

São comentário de coisas para ainda fazer no código, é uma forma que alguns programadores se organizam. Porem ele alerta que precisam ser apagados após a criação da funcionalidade e ainda sim quando fizer tem que estar de forma clara para outras pessoas entenderem o que será feito.

Comentário destaque, pode-se usar comentário para estacar algo importante.

<h2 align="center"> 🔹 Comentários ruim?</h2>

O autor  classifica alguns tipos de comentários ruins e informa que a maioria dos comentários e sua razão de existência entra nessa parte.

Comentário murmúrio, quando o programador acha que deve comentário, por desejo próprio colocando com suas próprias palavras não sendo claro. 

Comentários redundantes, comentários que explicam o que a função faz, porem a função ja é autoexplicativa. Outra situação é estar repetindo a mesma ideia, por exemplo 


```
//name
private String name
```

Comentários enganadores, como dito no inicio são casos de comentários que dizem uma coisa e a função ou trecho de código faz outra.

Comentário em final de chaves {} as vezes alguns programadores colocam o comentário no fechamento da função, algo muito ruim porque interfere no entendimento da função.

Comentário de créditos, alguns casos programadores colocam como comentário o nome de quem desenvolveu o código. Segundo o autor isso é péssimo.

Códigos como comentário, bem essa parte é quando você coloca trecho do código como comentário, seja no ato de debugar ou fazer o código e esquece de tira-lo depois. Deixar o código comentádo segundo o autor é a pior prática

## Frase impactante 

<i> "Não insira comentários em um código ruim, reescreva-o." pag 53 Clean Code </i>


### Breve entendimento do capitulo numero do capitulo do livro clean code