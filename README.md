# json-server CAPSTONE-ARTESA

## Endpoints

Assim como a documentação do JSON-Server-Auth traz (https://www.npmjs.com/package/json-server-auth), existem 3 endpoints que podem ser utilizados para cadastro, 2 endpoints que podem ser usados para login e 1 endpoint de produtos.

### Cadastro

POST /register <br/>
POST /signup <br/>
POST /users

Qualquer um desses 3 endpoints irá cadastrar o usuário na lista de "Users", sendo que os campos obrigatórios são os de email e password.
Você pode ficar a vontade para adicionar qualquer outra propriedade no corpo do cadastro dos usuários.
Exemplo de requisição para criação de usuários:

{
"email": "kenzinho@mail.com",
"name": "Kenzinho",
"password": "123456",
"state": "São Paulo",
"city": "Bauru",
"id": 1
}

### Login

POST /login <br/>
POST /signin

Qualquer um desses 2 endpoints pode ser usado para realizar login com um dos usuários cadastrados na lista de "Users"

### Produtos

GET /products

Retorna um array de objetos com os produtos cadastrados no JSON server.

POST /products
Nesse endpoint se realiza o cadastro de produtos para a venda, amarrado com o vendedor, para uso da localização.
=> "img" é opcional.

Exemplo de cadastro de produtos
{
"name": "Banana",
"category": "Frutas",
"price": 1.99,
"img": "https://static9.depositphotos.com/1642482/1149/i/950/depositphotos_11490585-stock-photo-bananas.jpg"
}
