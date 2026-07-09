Rest API com Python (Backend Completo)
---

O que é o FastAPI, conforme descrito em vídeo o FastApi, é uma como se fosse *"A estrutura do Python, que permite construir a parte de Backend de um site"*.

No caso da `"Framework"` do FastApi, ele cria os nomeados de end-points, de um site que basicamente é o link de um site sucedido de `/endpoin`, na prática, e como se tivéssemos o link do site para o sistema a ser construído, e pegássemos um método ou para fazer uma determinada coisa, o FastAPI, constrói a documentação dessa API, seguindo alguns preceitos que serão vistos posteriormente.

Outro ponto importante que foi apresentado na aula, é que através do FastAPI, é possível realizar o teste dos endpoint do site (a partir daqui os `endpoint's` serão denominado de links do site.), conforme demonstrado abaixo:    

> <table style="text-align: center; width: 100%;"> 
> <tr>
> <td style="text-align: center;">
> <img src="imgs/teste_endpoint_preview.png" alt="pd_info" width="50%"/>
> </td>
> </tr>
> </table>

---

## Sobre o projeto
O projeto que será desenvolvido terá como objetivo criar uma API utilizando o FastAPI,com os links do site, devidamente documentos e executáveis.  
Mais especificamente nesse projeto será criado todas as rotas (Links do site), assim como todas as funcionalidades correspondentes.

### Divisão do projeto de curso.

Para que um projeto em `FastAPI` possa funcionar corretamente recomenda-se que ele tenha uma certa divisão em seus arquivos do projeto, onde um tenha um arquivo de `main`, esse arquivo tem como objetivo criar o `FastAPI`, definir suas configurações tais como questões de criptografia e define-se as rotas da sua API.
> OBS: As rotas ou endpoint's de uma API nada mais são que o endereço final do site.  
Para além do que fora descrito acima faz-se necessário também que tenhamos criado dentro do projeto os arquivos de rotas, que nada mais é que os arquivos onde estarão presentes as configurações dos endpoint's.  
Porém para tudo que isso funcione conforme esperado precisamos de outros arquivos/modelos que auxiliem nesse projeto, sendo eles:  
- 1º Banco de dados.
- 2º Um arquivo de models
  - > Esse arquivo nada mais é que um meio de definir quais serão as tabelas do banco de dados.
- 3º Um arquivo de dependências.
  - > Essse arquivo é responsável por permitir algumas configurações, sejam de somente usuários autenticados realizarem certas ações, definições de ordem nas requisições etc..
- 4º Um arquivo de Schemas
  - > Esse arquivo é responsável por criar as estruturas padrões do `FASTAPI` para que possamos ter um processo mais eficiênte.
---

Diferentemente do comportamento padrão do `Python` no qual temos uma linguagem de programação que não é tipaada, ou pouco tipada, o `FastAPI` exige em sua utilização uma definição dos tipos das variáveis, por mais que esse tipo de escrita seja maior isso permite maior agilidade no processamento do `FASTAPI`, pois ele já espera que certas coisas sejam de um tipo determinado por exemplo, torando assim também com que a execução do projeto seja mais leve e performático. 

---

