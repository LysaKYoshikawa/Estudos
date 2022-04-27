<h1 align="center"> 📘 Funções</h1>

Conceitos e entendimentos do livro Clean Code - Resumo dissertativo 

Esse capítulo explica como escrever bem funções de forma claras. Ele descreve como podemos fazer isso e traz algumas reflexões do dia a dia.

Indice 
<p align="center">
 <a href="#As consequências de um código ruim">subtitulo</a> •
 <a href="#igualdade">subtitulo</a> • 
 <a href="#condicionais">subtitulo</a> • 
 <a href="#lacos">subtitulo</a> • 
 <a href="#Autor do quadro/livro">subtitulo</a>
</p>

<h2 align="center"> 🔹 Funções</h2>

As funções são a primeira linha de organização em qualquer programa.
Uma reflexão que o autor trás é que uma função tem que ser como um trecho de uma historia, ou seja a forma como você irá ler o código tem que seguir uma coerência e estar claro como uma narrativa.

<h2 align="center"> 🔹 Pequenas</h2>

Não tem uma pesquisa e nem referências que afirmam que funções pequenas são melhores, porém segundo o autor pela experiência dele quanto menor uma função, mais fácil de ler ela será. 
Isso não quer dizer que caso ocorra a necessidade da função ser grande, que o codigo está ruim, mas que irá requer mais esforço para entender ela.

O autor informa que em meados de 1980 era comum dizer que uma função não podia passar do tamanho da tela do monitor. Naquela época as telas comuns para programação eram VT100, de 24 linhas. Atualmente com fontes reduzidas e monitores grandes fácilmente em uma tela passaria de 100 linhas, porém o mesmo afirma que uma função jamais deve chegar a tanto, as funções devem ter no máximo 20 linhas 

<h2 align="center"> 🔹 Blocos e indentação</h2>

Aqui trás intruções que blocos como: ```If, else, while ``` e outros devem ter apenas uma linha, usando um ternário por exemplo. É explicado também que o nivel de indentação deve ter no máximo 1 ou 2 espaços  o que o que acaba influênciando para a função ser pequena.


<h2 align="center"> 🔹 Objetividade </h2>

As funções precisam fazer apenas uma coisa simples. Isso que dizer que uma função que executa mais de uma objetividade, mais de uma coisa a função corre o risco de perder-se na sua funcionalidade, fica mais propenço a bug e alem de ficar mais difícil de entender a função.

Mas não é apenas fazer uma coisa é fazer ela bem feita e de fato executar essa ```uma coisa```.

Pensei um exemplo para entender essa parte.Imagine uma pessoa, saindo de casa,com os seguintes trajes: 
touca,
camiseta regata,
sobretudo no braço,
short,
sem sapatos,
meias de dinossauro ate o joelho e 
de luvas.
Essa pessoa sai de casa vestida desse jeito.

Você não consegue por esses trajes determinar se a pessoa saiu para um dia ensolarado, um dia de frio ou chuvoso. Uma função que executa várias coisas, seria como uma pessoa que não sabe a roupa que vai usar. Imagine que essa pessoa esta saindo para uma cidade onde o clima é abaixo de 0°c a probabilidade dela adquirir uma gripe é grande, essa "gripe" poderia ser um bug ou uma interpretação errada da função.

O mais difícil é entender o que seria essa ```uma coisa``` uma forma que o autor tras de dica é listar o que a função esta fazendo e se chegar em alguma parte do código que você consegue abstrair e fazer uma função dessa abstração, então talvez seja uma opção, quebrar a função em mais de uma.

Outro ponto importante que o autor tráz é que ao fazer uma lista pode-se entender que a função esta fazendo varias coisas e assim entender que está construindo errado a função. Entretanto se a função está seguindo um passo à passo para uma mesma finalidade ou ```uma mesma coisa``` então a função esta seguindo a regra da objetividade. 

<h2 align="center"> 🔹 Regra decrescente </h2>

Regra decrescente é ler o código de cima para baixo, como uma narrativa. Que cada função seja seguida pelas outras no próximo nível de abstração de modo que possa ser lido descendo o nível de abstração.

Segundo o autor: "Acaba sendo muito difícil para os programadores aprenderem a seguir essa regra e criar funções que fiquem em apenas um nível de abstração. Mas aprender esse truque é tambem muito importante , pois ele é o segredo para manter as funções curtas e garantir que façam apenas uma coisa". pág 37

<h2 align="center"> 🔹 Switch </h2>

É difícil fazer um switch que faz apenas uma coisa, via de regra um ```switch``` faz ```N``` coisas.
O autor tráz como dica para usar o polimorfismo, deixando o switch em uma classe de baixo nivel e garantindo que nunca é repetido.

No livro ele tras um exemplo em java

```
public Money calculatePay(Employee e)
throws InvalidEmployeeType{
    switch(e.type){
        case COMMISSIONED:
        return calculateCommisionedPay(e);
        case HOURLY:
        return calculateHourlyPay(e);
        case SALARIED:
        return calculateSlariedPay(e);
        default:
        throw new InvalidEmployeeType(e.type)
    }
}
```
Aqui o autor trouxe 4 pontos negativos a esse exemplo.

- Primeiro ela é muito grande
- Segundo ela faz mais de uma coisa
- Terceiro ela viola o Princípio da Responsabilidade Unica(SRP) por haver mais de um motivo para altera-la
- Quarto ela viola Princípio de Aberto-Fechado (OCP), pois será necessário modifica-la sempre que novos funcionários entrarem

Ele diz que switch são aceitas se aparecerem apenas uam vez, como para criação de objetos poliformicos, e estiverem escondidas atras de uma relação de herança de modo que o resto do sistema não terá acesso. Porém claro que tudo tem uma excessão e pode haver momentos que não dará para seguir todas as regras.

<h2 align="center"> 🔹 Nomes de funções</h2>
Outra dica que ele tras para funções claras seria usar nomes descritivos. Nomes que trazem o que realmente a função esta fazendo.
Claro que muitas vezes ao escolher um bom nome talvez seja necessário uma refaturação no código, porque será o momento que possivelmente você irá enxergar pontos de melhoria.

Escolher um bom nome pode ir desde explicar o que a função faz à explicar e ordenar a finalidade dos parâmetros. Por exemplo uma função mônade(função onde existe um parâmetro), em uma função desse tipo o parâmetro e o nome da devem formar um par. Por exemplo ```write(name)``` esta bem claro pelo nome, a sua finalidade.

<h2 align="center"> 🔹 Parâmetros de funções</h2>

Parâmetro é o nome que damos para a variável que declaramos, com objetivo de retornar o valor da função.

Segundo clean code a quantidade ideal para ter de parâmetros numa função é zero. Depois é com um parâmetro chamado mônade, depois com dois parâmetros chamada de díade e por último triáde com três parâmetros. Acima de três parâmetros conhecida como políade, deve haver um motivo específico para a sua existência então o ideal seria rever a lógica e procurar uma construção melhor.

Uma função com zero parâmetro ou função mônade é simples de entender o objetivo, e ate de escrever testes para função fica mais prático. Uma função díade e tríade exige mais atenção ao código e entender o que ele esta fazendo.

Funções díades com dois parâmetros e tríades de três parâmetros, são mais difícieis de entender, exemplo se ler ```function write(name)``` só pelo nome consegue entender o objetivo da função, agora ler ```function write(output-Stream, name)```, acrescenta um nível de complexidade para entendimento da função e quantos mais parâmetros mais complexo fica o entendimento da função.

Um ponto importante que o autor tráz também, que caso necessário ter mais de um parâmetro em uma função, é importante que elas tenham o mesmo objetivo. Ou seja, ter funções com parâmetros de objetivos tão distintos, pode confundir a sua interpretação e objetividade. Exemplo ```function sendMail(stageError, writeEmail, document)``` é como ter três atores principais agindo ao mesmo tempo, não tem como saber quem é quem de forma clara, sem ter que ler o código. 


<h2 align="center"> 🔹 Objetos como parâmetros</h2>
Uma solução que o autor tras para casos que tenham vários parâmetros é colocar alguns deles dentro de uma classe própria ou transformando eles em objetos, desde que seguem o mesmo sentido. 

```
const emailStage = {
  "PREPARAÇÃO DOCUMENTAL": "oneStage.html",
  "EM ANÁLISE": "twoStage.html",
  "ADEQUAÇÕES FÍSICAS": "treeStage.html",
  "EM COMUNIQUE-SE": "fourStage.html",
  "AGUARDANDO VISTORIA": "fiveStage.html",
  "OBTIDO": "sixStage.html",
};
```


<h2 align="center"> 🔹 Efeitos colaterais</h2>

Efeitos colaterais são mentiras. Uma função promete fazer uma coisa porém ela tambem faz outra coisa.
Algo que pode ser um problema conforme for crescendo a complexidade do código e as implementações.
As funções devem fazer uma coisa e ter um objetivo. Se ela fazer alguma coisa escondida pode gerar efeitos colaterais, que resultam em acoplamentos temporarios estranhos e dependências.

O autor traz um exemplo de uma função chamada ```checkPassword``` segundo o nome ela verifica a senha. Porém vamos supor que a função também inicia sessão, algo que está dentro da função que para entender precisa ler e identificar no código.


<h2 align="center"> 🔹 Tratamento de erros</h2>

Tratamento de erros é algo específico e único, ou seja uma coisa só. Sendo assim uma função que trata de erros deve fazer apenas isso.

Blocos como ```try/cath``` quando estão dentro de uma função, misturada com o objetivo de outra parte do código pode confundir a estrutura e o processamento normal do código, sendo assim nesses casos é importante serem extraídos para uma função própria.

Concluíndo....

Escrever uma função é pensando para outra pessoa ler, precisa ser algo que seja tranquilo e menos frutante o livro tenta trazer dicas e formas de fazer isso.

### Breve entendimento do capitulo 3 - Funções do livro Clean Code.