<h1 align="center"> 🎡 Nomes significativos</h1>

<div align="center">

   ![image](https://user-images.githubusercontent.com/64383080/161648241-61c6f926-f548-412a-a3c8-743c91229758.png)

   Conceitos e entendimentos do livro Clean Code - Resumo dissertativo 

</div>


 
<p align="center">
 <a href="#">Porque Escolher bons nomes</a> •
 <a href="#">Dicas e Reflexões sobre nomes</a> • 
 <a href="#">Nome de classes</a> • 
 <a href="#">Nome de Métodos</a> • 
</p>

Se analisar um programa nomeamos tudo, desde funções, variáveis a pacotes e codigos fontes. Mas quantas vezes ao entrar em um código percebemos que o nome da função não condizia com a sua funcionalidade.

<h2 align="center"> 🔹 Porque escolher bons nomes</h2>

Depois de ler o capítulo tive uma interpretação própria da sua importância. Bons nomes podem trazer clareza ao que trata-se o determinado trecho de código. 

Imagine que você não pode ver um objeto e nem tocá-lo. Porém, alguém te fala que esse objeto se chama `vdFlor` e disseram que você precisa levar para a `JTS`. Ai depois de muito tempo, mas muito tempo, você entende que `vdFlor` trata-se de um `vaso de flor` e `JTS` trata-se de ir a `janela tomar sol`.

Um código mal nomeado trata-se exatamente dessa situação é algo que não esta claro é você não consegue ver.




<h2 align="center"> 🔹  Dicas e reflexões sobre nomes</h2>

Abaixo tem uma série de reflexões que o autor abordou para pensar em bons nomes e sugestões de como poderia dar bons nomes.

<h3 align="center"> 🔸  Distinções sobre os nomes</h3>
 Um ponto que o autor tráz é fazer distinção no nome, mesmo sendo coisas parecidas elas tem funcionalidades distintas.

 Um exmeplo que foi abordado foi:

 `getActiveAccount()`;

 `getActiveAccounts()`;

 `getActiveAccountInfo()`;

São nomes parecidos para situações diferentes, então detalhar ou diferenciar elas é importante, porque caso contrário como saber qual função chamar?

Ou outras situações como nomear `e1` `e2` e `e3`. Essa situação também não está clara.
Outro ponto que o autor tambem tras é evitar codificar em nomes colocar ou reduzir nomes para uma letra.

<h3 align="center"> 🔸 Nomes que revelam propositos</h3>

Um ponto que o autor trás 


<p> <i>"O nome de uma variavel, função ou classe deve responder a todasas grandes questões. Ele deve lhe dizer porque existe o que faz e como é usado"- pag 18 Clean Code </i> </p>

Ele ainda trás um ponto que se o nome escolhido necessita de um comentario para explicar ele, significa que o nome não é um bom nome.
No capítulo o autor tras uma reflexão com um código, cujo o nome das variaves e funçãoes não traziam um conceito para aquela função. Vou trazer um exemplo de um codigo proprio 
```
 @RequestMapping("/vagas")
    public ModelAndView listaVagas(){
        ModelAndView mv = new ModelAndView("relatorio");
        Iterable<Vaga> vagas = vr.findAll();
        mv.addObject("vagas", vagas);
        return mv;
    }

```
vr vem de outro trecho de codigo que não esta claremente especificado. 
e não se tem claremente a ideia do que trata-se o código. Tendo que procurar da onde vem algumas denominações para entender seu sentido.

Uma dica que ele tras para pensar na objetividade do nome é respopnder as perguntas:

- Qual a importância dessa função/variavel....?
- O que essa funcionalidade faz? ou o que esse trecho de codigo faz?

<h3 align="center"> 🔸 Palavras que dão outro sentido</h3>

Outro ponto que o autor tras também é evitar nomear com siglas ou palavras que podem confundir a interpretação. Exemplo é o `accountList`, porque lista para programadores significa algo especifico, então nesse caso poderia ficar bem denominado `account` ou `accountGroup`.

Assim como usar nomes muito parecidos exemplo: 

```
 const ABCNomeDeVarivel
 const ABCNomeDeVariaveis
```
Por serem nomes muito parecidos fica confuso a interpretação e facilcimente de relacionar alguma funcionalidade ao nome errado tambem.

<h3 align="center"> 🔸 Nome pronunciavel</h3>

Se você planeja nomear algo precisa ver se quem irá ler conseguirá ler o nome. 
Ele trouxe uma situção que tinha uma variável com o nome `genymdhms` <i> (generation date, year, month, day, hour, minute e second) </i>, não tem como entender do que trata-se esse nome e nem de pronuncia-lo para perguntar ao colega.

<h3 align="center"> 🔸 Nome facil de buscar</h3>

Como já foi falado nomes com um número, ou uma letra, não são fáceis de buscar, imagina procurar um nome `A` como variável. 
Porem existe momentos que podemos usar nomes com uma letra quando estão dentro de metodos pequenos por exemplo o `for`, desde que se limite a um uso dentro do metodo, caso ele seja repetitivo ou usado em varios lugares é impresindivel nomear de forma clara e sucinta nesse caso.

<h3 align="center"> 🔸 Nomes do dominio da solução</h3>

Outra dica importante que o autor traz é que caso não consiga de nenhuma forma nomear o arquivo pense no nome do dominio do problema. De fato saber que o nome não está bom e pensar em um nome bom é dificil então ele passa essa dica caso não consiga pensar em nenhum nome a <i>la programador</i>. 

<h3 align="center"> 🔸Contexto no nome </h3>

Um nome como `message` pode não ser claro, afinal não dá para saber do que trata-se esse nome, então dar um contexto ao nome tambem é importante como `massageBox`. 
Outro exemplo é variaveis de endereço como lastName, street, houseNumber, state...Se elas estiverem juntas será facil presumir que trata-se de um endereço, porem se aparecer `state` no meio do código fica difícil entender do que ele se refere. Então nesse caso adicionar um contexto como `addrState` pode ficar mais claro.

Porém, também reflete pensar no contexto desnecessário como sigla da empresa nome da variável, isso não é prático e não é legível. Exemplo: Estado de São Paulo e variavel `SPAddress`

<h2 align="center"> 🔹  Nomes de classes</h2>

Classes e objetos devem ter nomes com substantivos como Custumes, WikePage, Account e AddressParser 

<h2 align="center" #condicionais > 🔹  Nomes de métodos</h2>

Os nomes de métodos devem ter verbos, como `Post Payment` , `Delete Page` ou `Save`


## Frase impactante 

<i> "Uma diferença entreum programador esperto e um programador profissional é que este entende que clareza é fundamental. Os profissionais usam seus poderes para o bem e escrevem códigos que outros possam entender." pag 25 Clean Code </i>

### Breve entendimento do capitulo 2 do livro clean code

