# Projeto API CRUD com Java e Spring Boot

Este é um projeto de API RESTful desenvolvido em Java com o framework Spring Boot. A API permite realizar operações CRUD (Create, Read, Update, Delete) em uma entidade de produtos.

## Funcionalidades

- Cadastro de um novo produto
- Busca de todos os produtos cadastrados
- Busca de um produto específico por ID
- Atualização de um produto existente
- Remoção de um produto pelo seu ID

## Tecnologias Utilizadas

- Java
- Spring Boot
- Spring Data JPA
- PostgreSQL (banco de dados relacional)
- Maven (para gerenciamento de dependências e build)

## Configuração do Ambiente de Desenvolvimento

1. Clone este repositório para o seu ambiente local:
```
   https://github.com/JoneilsonLima/api-produtos.git
```
2. Importe o projeto para sua IDE.

3. Certifique-se de que todas as dependências do Maven foram baixadas.

## Executando a Aplicação

1. No diretório raiz do projeto, execute o seguinte comando:
```
mvn spring-boot:run
```
2. A aplicação será iniciada e estará disponível em `http://localhost:8080`.

 ## Endpoints da API

- `GET /products`: Retorna todos os produtos cadastrados.
- `GET /products/{id}`: Retorna um produto específico pelo seu ID.
- `POST /products`: Cria um novo produto.
- `PUT /products/{id}`: Atualiza um produto existente pelo seu ID.
- `DELETE /products/{id}`: Remove um produto pelo seu ID.

## Exemplo de Requisição e Resposta
### Requisição POST /products

POST /products
Content-Type: application/json
```
{
  "name": "Produto A",
  "value": 29.99,
}
```

