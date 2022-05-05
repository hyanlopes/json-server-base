# json-server-base

Esse é o repositório com a base de JSON-Server + JSON-Server-Auth já configurada, feita para ser usada no desenvolvimento das API's nos Capstones do Q2.

## Endpoints

Assim como a documentação do JSON-Server-Auth traz (https://www.npmjs.com/package/json-server-auth), existem 3 endpoints que podem ser utilizados para cadastro e 2 endpoints que podem ser usados para login.

### Cadastro

POST /register <br/>
POST /signup <br/>
POST /users

Qualquer um desses 3 endpoints irá cadastrar o usuário na lista de "Users", sendo que os campos obrigatórios são os de email e password.
Você pode ficar a vontade para adicionar qualquer outra propriedade no corpo do cadastro dos usuários.

### Login

POST /login <br/>
POST /signin

Qualquer um desses 2 endpoints pode ser usado para realizar login com um dos usuários cadastrados na lista de "Users"

### Animais

POST /animais <br/>

Este endPoint ira cadastrar um animal, voce precisa ter em mãos o token para cadastro e o seu id de usuário dado no login ou cadastro.

GET /animais <br/>

Este endPoint é responsavel por listar todos os animais, você precisa ter um cadastrado na sua conta para ter acesso aos outros, precisa também do seu token.

### infoAnimais

GET /infosAnimais <br/>

Este endPoint é responsavel por mostrar dicas e cuidados para seu pet, somente pessoas cadastradas conseguem ver, tenha em mãos seu token. Ah e não é possivel editar-lo!
