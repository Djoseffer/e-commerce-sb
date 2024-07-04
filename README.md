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

```bash
spring.datasource.url=jdbc:mysql://localhost:3306/coursesb
spring.datasource.username=root
spring.datasource.password=root
spring.jpa.properties.hibernate.jdbc.lob.non_contextual_creation=true
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.jpa.properties.hibernate.format_sql=true
```bash

Executar a aplicação:

Execute a classe principal Application.java como uma aplicação Spring Boot.

````
mvn spring-boot:run
````
