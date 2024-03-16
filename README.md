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

- `POST /api/posts`: Cadastra um novo post.
- `GET /api/posts`: Retorna todos os posts.
- `GET /api/posts/${postId}/${likedPost}`: Busca o post por id passando um outro parámetro se está no visualizando no feed ou perfil.
- `PUT /api/posts/${postId}/like`: Curti um post.
- `GET /api/posts/search/${name}`: Busca post pelo nome.
- `POST /api/comments/create`: Cadastra um comentário em um post.
- `GET /api/comments/${postId}`: Busca todos os comentários de um post.

## Exemplo de Requisição e Resposta
### Requisição GET /api/posts

GET /api/posts
```
[
   {
       "id": 2,
       "name": root,
       "content": exemplo,
       "postedBy": jhon,
       "img": "https://images.com/",
       "date": "2024-03-14T04:03:26.854+00:00",
       "likeCount": 12,
       "viewCount": 30,
       "tags": [
          "neve",
          "férias"
       ]
   }
]
```

