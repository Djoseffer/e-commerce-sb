# Sistema de Pedidos Online

## Descrição

O Sistema de Pedidos Online é uma aplicação Java desenvolvida utilizando o framework Spring Boot com integração ao banco de dados MySQL. Ele gerencia pedidos de clientes, incluindo categorias de produtos, detalhes de pedidos, pagamentos e itens de pedido.

## Instruções de Instalação e Pré-requisitos

Antes de iniciar, certifique-se de ter as seguintes ferramentas instaladas:

- JDK 11 ou superior
- Maven
- MySQL Server

### Instalação

1. **Clonar o repositório:**

   ```bash
   git clone https://github.com/seu-usuario/nome-do-repositorio.git
   cd nome-do-repositorio
  ```bash


Configurar o banco de dados:

Crie um banco de dados MySQL com o nome coursesb (ou o nome que preferir).

Configure as credenciais de acesso ao banco de dados no arquivo application.properties

```
```bash
spring.datasource.url=jdbc:mysql://localhost:3306/coursesb
spring.datasource.username=root
spring.datasource.password=root
spring.jpa.properties.hibernate.jdbc.lob.non_contextual_creation=true
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.jpa.properties.hibernate.format_sql=true
Executar a aplicação:

````
Execute a classe principal Application.java como uma aplicação Spring Boot.


```bash
mvn spring-boot:run
```

Como Utilizar
Endpoints da API
A API possui os seguintes endpoints principais:

Clientes:

GET /users: Retorna todos os usuários cadastrados.
GET /users/{id}: Retorna um usuário específico pelo ID.
POST /users: Cria um novo usuário.
PUT /users/{id}: Atualiza um usuário existente.
DELETE /users/{id}: Remove um usuário pelo ID.
Categorias:

GET /categories: Retorna todas as categorias de produtos cadastradas.
GET /categories/{id}: Retorna uma categoria específica pelo ID.
Pedidos:

GET /orders: Retorna todos os pedidos cadastrados.
GET /orders/{id}: Retorna um pedido específico pelo ID.
Produtos:

GET /products: Retorna todos os produtos cadastrados.
GET /products/{id}: Retorna um produto específico pelo ID.
Exemplos de Requisições
GET /users

```bash
GET /users HTTP/1.1
Host: localhost:8080
```
```bash
[
    {
        "id": 1,
        "name": "João",
        "email": "joao@example.com",
        "phone": "(11) 99999-9999"
    },
    {
        "id": 2,
        "name": "Maria",
        "email": "maria@example.com",
        "phone": "(11) 88888-8888"
    }
]
```
POST /users
```bash
POST /users HTTP/1.1
Host: localhost:8080
Content-Type: application/json

{
    "name": "José",
    "email": "jose@example.com",
    "phone": "(11) 77777-7777",
    "password": "senha123"
}
```



