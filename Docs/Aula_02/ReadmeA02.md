# Requisições e Roteamento da API

---
## Criando rotas para nossa API

Com os processos realizados anteriormentedaremos continuidade em nosso projeto, nesse tópico iremos abordar como realizamos a confecção de rotas para nossa API.  
Na aula passada paramos exatamente no ponto de inicialização nossa aplicação instanciando na variavel o objeto `FASTAPI()`. 
Mas antes de realizarmos o Deploy da aplicação em um dóminio ou algo ddo tipo precisamos realizar a definição das rotas ou dos `endpoint's` dessa aplicação, essas rotas ou endoints nada mais são que o final do site que será ajustado em nossas rotas.  
E importante que tenhamos essas rotas definidas e configuradas pois através delas que iremos definir, quais serão as funcionalidades do nosso sitema, e cada saída pode ter um tipo de requisição possível, sendo elas:  
> - Get (Leitura/Pegar informações presentes no Site)
> - Post (Enviar/Criar informações)
> - Put/Patch (Atualizar/Editar informações presentes no SITE.)
> - Delete (Deletar informações presente)
> Esses tipos de requições são nada mais que um CRUD.

Esse tipo de utilização em API's são conhecidas como REST API, ou seja para cada endpoint e determinado qual será o tipo de requisição a ser feita, o padrão de uma `REST API` consite em realizar chamadas nas rotas e devolvelas com o formato `Json`, nesse módulo iremos incrementar nosso projeto criando as principais rotas para cada tipo de chamada.
Em muitas API'S somente trabalham com 2 tipos de requisições post get, e em nosso projeto também iremos realizar esse processo principalmente nas requisições de put/patch através da rota do post,pois esse tipo de rota já realiza um tipo de edição seja para criar algo ou editar algo que já existe.  

Quando desejamos criar um novo ENDPOINT nada mais é que criar o que ficara após o nosso dóminio do site, ou seja no caso localhost/ordens, será criado o caminho + o tipo de requisição que esse ENDPOINT receberá. 

---

Para o nosso projeto em questão adotaremos uma das 3 possíbilidas de criação de rotas, essas podem ser tanto dentro do proprio arquivo da main (o que por mais que seja uma API simples não é o recomendado), ou podemos criar um novo arquivo chamado de `routers.py` e dentro desse arquivo conter todas as rotas, ou ainda a 3ª opção que essa será a adota uma terceira opção, que será realizar a divisão por sessões, ou seja teremos 2 arquivos diferentes uma para autenticação e outro para os pedidos.