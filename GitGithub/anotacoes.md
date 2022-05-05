
<h1 align="center"> 📘 Git : controle e compartilhamento seu código</h1>

Conceitos e entendimentos do livro Clean Code - Resumo dissertativo 

indice 
<p align="center">
 <a href="#">Controle de versão ou Version Control System - VCS</a> •
 <a href="#">Quando commitar</a> • 
 <a href="#">Branch</a> • 
 <a href="#">Comandos</a> • 
 <a href="#">subtitulo</a>
</p>


<h2 align="center"> 🔹 Controle de versão ou Version Control System - VCS</h2>

VCS : É a ação de controlar a versão do código que será implementada e assim não subir versão de código desatualizada. Isso pode ocorrer quando você está trabalhando em time e várias pessoas desejam subir uma versão do código atualizado para um repositorio local.

Neste servidor, deve haver alguma ferramenta capaz de identificar que a versão enviada não é a mais recente, e portanto não deixe o arquivo ser enviado. Isto é, antes do envio de uma alteração, este colega de trabalho precisará baixar as alterações que já foram enviadas, para que só então consiga enviar a versão atualizada por ele.

- Nos ajudam a manter um histórico de alterações;
- Nos ajudam a ter controle sobre cada alteração no código;
- Nos ajudam para que uma alteração de determinada pessoa não influencie na alteração realizada por outra;

<h2 align="center"> 🔹 Quando commitar</h2>

Devemos gerar um commit sempre que a nossa base de código está em um estado do qual gostaríamos de nos lembrar. Nunca devemos ter commits de códigos que não funcionam, mas também não é interessante deixar para commitar apenas no final de uma feature.

<h2 align="center"> 🔹 Branch</h2>
Branches ("ramos") são utilizados para desenvolver funcionalidades isoladas umas das outras. A branch master é a branch "padrão" quando você cria um repositório.

É interessante separar o desenvolvimento de funcionalidades em branches diferentes, para que as mudanças no código para uma não influencie no funcionamento de outra.

<h2 align="center"> 🔹 Diferença de Merge e Rebase</h2>
O merge junta os trabalhos e gera um merge commit. O rebase aplica os commits de outra branch na branch atual.

https://medium.datadriveninvestor.com/git-rebase-vs-merge-cc5199edd77c

Com o `git checkout ` nós desfazemos uma alteração que ainda não foi adicionada ao `index ` ou `stage `, ou seja, antes do `git add `. Depois de adicionar com `git add `, para desfazer uma alteração, precisamos tirá-la deste estado, com `git reset `. Agora, se já realizamos o `commit `, o comando `git revert ` pode nos salvar.

<h2 align="center"> 🔹 Reverter um commit</h2>
Supondo que eu tenha dado um git add ., porém percebi que não era para subir como git add porque ainda tem ajustes, então desfazer esse commit você pode usar o comando 

`git reverse <numero da hash> ` posso desfazer um commit

primeiro tem que dar `git log` pegar o numero de `hash ` e colocar ele seguido o `git reverse ` .

![image](https://user-images.githubusercontent.com/64383080/166515918-cbda91df-7460-426b-95af-572c323a9109.png)

ele ira criar um commit de que foi desfeito o commit anterior.

<h2 align="center"> 🔹 E se eu quiser guardar um commit pra mexer depois?</h2>
Caso ocorra a situação que eu precise ir para outro projeto e queira salvar as alterações que fiz do código, porem ele ainda não esta funcionando conforme regras.

posso usar o comando `git stash ` conseguimos salvar todas as alterações,  para um local temporário, sem necessidade de um commit ou de se gerar um commit para isto.

 após `git stash ` executarmos `git stash list `, teremos uma lista de tudo que estiver salvo nestas condições. Como no exercicio em apenas uma alteração mostrara apenas uma alteração.

 ![image](https://user-images.githubusercontent.com/64383080/166567498-d593f127-a1ae-4736-b555-a69461332d55.png)


Supondo que você voltou a trabalhar no projeto fez alterações e fez commit delas e quero voltar a trabalhar com as alterações que estão no `stash `, podemos primeiro dar `git stash list ` verificar o numero da alteração e passar o comando `git stash apply 0 ` como no exemplo:  

![image](https://user-images.githubusercontent.com/64383080/166568163-7907ba1d-f267-4e9f-aab7-c33b35312d39.png)

Depois precisaria dar `git stash drop ` para remover as alterações 

![image](https://user-images.githubusercontent.com/64383080/166568397-924f1a3c-2674-460d-9850-f3a0174b5db7.png)

Outra forma de fazer seria pegar as alterações e execluir o item da list do stash, que dá para ser feito com `git stash pop `, ele realiza o merge com as modificações que já temos e aplica aquelas que já estavam salvas lá.

<h2 align="center"> 🔹 Viajar entre commits</h2>
Supondo que precisa voltar em algum commit, você precisa pegar o inicio da hash que esta abaixo na coluna amarela

![image](https://user-images.githubusercontent.com/64383080/166615212-3139173f-a4ed-47ff-948d-cce660e61cec.png)

e dar um comando `git checkout 6771525 ` esse numero na frente são os 7 primeiro digitos da identificação do commit, como eles são unicos basta dar essa sequência, que você ira para um commit anterior

Vai aparecer uma mensagem informando que você esta em um commit anterior que atualização atualizações posteriores a ela não estão nesse commit.

<h2 align="center"> 🔹 Comandos</h2>

`git init `  esse comando você inicializa o repositorio como se estivesse dizendo "aqui tem um repositorio"
`git status ` ele mostra tudo que foi alterado, incluído e excluído. Enfim todas as alterações do projeto

Os comandos abaixo é para o caso de ser o primeiro acesso ao git na sua maquina, então precisa colocar seu nome e seu e-mail.
```
git config --local user.name "Seu nome aqui"
git config --local user.email "seu@email.aqui"COPIAR CÓDIGO
```
`git add . ` você adiciona todas as alterações realizadas
`git add < nome do aquivo> ` ele sera add somente o arquivo que escreveu

`git rm ` ser para remover um arquivoe para que o mesmo deuxe de ser monitorado

`git commit -m ` você esta escrevendo do que trata-se o commit que é uma versão do seu código que esta sendo subido. ```-m``` serve para passarmos uma mensagem de commit, que serpá incluído entre aspas.

`clear ` é para limpar a tela

`HEAD ` : Estado atual do nosso código, ou seja, onde o Git os colocou

`Working tree `: Local onde os arquivos realmente estão sendo armazenados e editados

`index `: Local onde o Git armazena o que será commitado, ou seja, o local entre a working tree e o repositório Git em si.

`git log ` você pode verificar o historico das alterações 

`hash do commit ` é uma identificação única de  cada commit, isto é não existem dois commits com o mesmo hash. O condigo grifado de amarelo é o hash

![image](https://user-images.githubusercontent.com/64383080/165326882-c7f4c279-cd6d-4266-a1ac-e5e48c9c9a4f.png)

`git config --local ` você realiza as alterações o config te permite configurar.

`git log --oneline ` traz os historicos de alterações resumidos 
Caso entre no log e não consiga mais sair aperte a tecla `q`

`git log -p ` tras mais informações, como as alterações do commit.

`git log --pretty="format:%H" `, comando traz apenas o hash

`git log --pretty="format:%h %s" `, por sua vez traz o hash resumido seguido pela mensagem do commit

`git log --help ` da para ver algumas das opções possiveis para o uso do git log. Tambem tem o link mostrando outras opções https://devhints.io/git-log

`gitignore ` é um arquivo que vem junto ao seu repositorio. Ele serve para controlar os arquivos que não serão monitorado. Exemplo supondo que você tem um arquivo que não deseja ser monitorado, então você pode colocar esse arquivo dentro do gitignore e ele não sera monitorado
![image](https://user-images.githubusercontent.com/64383080/165366335-306522b7-1d9a-42df-9f7f-8505992f889c.png)

`git init --bare ` significa que esse repositorio é um repositorio puro só contem as alterações dos arquivos não contém uma cópia de cada arquivo.

Para eu fazer um repositorio que eu ja tenho reconhecer o repositorio que criei com git init --bare vou usar o comando git remote e depois git e remote add local e o endereço. exemplo:

![image](https://user-images.githubusercontent.com/64383080/165838152-95accbbc-e584-4ba6-9657-f801dc15784b.png)

Depois pode dar o comando git remote local para ele listar 

Depois `git remote -v ` 

![image](https://user-images.githubusercontent.com/64383080/165838390-71b30da1-b7dd-43b2-a717-f8165b27e69a.png)

Em situações complexas, de uma infraestrutura de redes mais robusta, poderíamos fazer o envio para um local e a busca viria de outro. Não é nosso caso, portanto não nos preocuparemos com isto no momento. Já criamos um repositório remoto, que adicionamos no repositório local, e agora passaremos a imaginar que a Ana está trabalhando conosco e precisa baixar os dados contidos neste repositório.

Voltaremos à pasta `git-e-github` por meio de `cd .. `, e criaremos uma pasta para a Ana, com mkdir ana. Acessaremos a pasta com cd ana, e ela então precisará clonar o repositório, é assim que chamamos quando queremos trazer todos os dados de um repositório remoto para o nosso repositório local pela primeira vez.

Sendo assim, executaremos `git clone /c/Users/ALURA/Documents/git-e-github/servidor `, para que sejam trazidos os dados do repositório localizado neste endereço. Isso fará com que dentro da pasta "ana" seja criada uma pasta chamada "servidor". Porém, não é o que queremos; queremos que a pasta seja "projeto", por exemplo, e para isso executaremos `git clone /c/Users/ALURA/Documents/git-e-github/servidor ` projeto.

Após "Enter", somos informados de que o clone foi realizado, mas há um aviso de que o repositório clonado está vazio. Mas não adicionamos o repositório remoto no repositório do Vinicius? Sim, porém não enviamos os nossos dados para ele! Portanto, a Ana não possui acesso a eles, e é por isto que o repositório dela está vazio. A seguir, entenderemos como enviar dados para um repositório e buscar as suas modificações.

com ```git init --bare``` Com este comando nós criamos um repositório que não terá a working tree, ou seja, não conterá uma cópia dos nossos arquivos. Como o repositório servirá apenas como servidor, para que outros membros da equipe sincronizem seus trabalhos, poupamos espaço de armazenamento desta forma.


Antes de sincronizar as nossas mudanças no código com algum repositório remoto, precisamos adicioná-lo ao nosso repositório local.
Como adicionamos esta ligação entre os repositórios?
```git remote add nome-repositorio caminho/para/o/repositorio```
Desta forma teremos um link do nosso repositório local com o repositório remoto, que chamamos de nome-repositorio, que está armazenado em caminho/para/o/repositorio.

`git remote rename ` ele renomeia o repositorio

`git oringin -p ` vai mostrar a atualização

`git pull ` vai atualizar o código.




### Breve entendimento do capitulo numero do capitulo do livro clean code