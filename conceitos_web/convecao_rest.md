
Dentro do protocolo de apis temos apis soap e rest

Nas conveções rest temos os caminhos 

URL   | Metodo | Descrição
--------- | ------ | ------ 
/clientes | POST | inclui novo cliente
/clientes | GET | obtem todos os clientes
/clientes/id&36 | GET | Obtem especificamente o cliente de id 36
/clientes/id&12  | PUT | Atualiza cliente do id 12
/clientes/id&59  | DELETE | Exclui o cliente de id 59 

Existe duas arquitetura SOA e MicroServicos

SOA = é uma arquitetura mais antiga cerca de 15 anos. Você tem que ter um software que é o SB Enterprise Service busca o barramento e nesse software você

vai instalando seus serviços e depois que o seu serviço está instalado você vai fazer depois lá por

exemplo medir fluxos que vão usar esse serviço para fazer algum tipo de trabalho.

MicroServiços =
Por outro lado você tem arquitetura de micro serviços que são sistemas Micro Sistemas bastante especializados

que ciclo de vida própria sua linguagem de programação própria e seu banco de dados próprio.

Via de regra você pega um servico e quebra ele em varios serviços e tem um time 