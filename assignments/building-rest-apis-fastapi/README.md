# 📘 Assignment: Building REST APIs with FastAPI

## 🎯 Objective

Aprenda a criar uma API REST com FastAPI, definindo endpoints, validando dados com modelos Pydantic e retornando respostas HTTP apropriadas. Ao final, você terá uma API de catálogo de livros documentada e coberta por testes básicos.

## 📝 Tasks

### 🛠️ Criar os primeiros endpoints

#### Descrição
Configure uma aplicação FastAPI para gerenciar um catálogo de livros em memória. Crie endpoints para consultar os livros cadastrados e adicionar um novo livro.

#### Requisitos
O programa concluído deve:

- Instalar FastAPI e Uvicorn e iniciar a aplicação com `uvicorn main:app --reload`
- Criar um modelo Pydantic para os dados de entrada de um livro, incluindo título e autor
- Implementar `GET /books` para retornar a lista de livros e `POST /books` para adicionar um livro
- Gerar um identificador único para cada livro criado e retornar o livro adicionado na resposta
- Disponibilizar a documentação interativa da API em `/docs`


### 🛠️ Implementar operações CRUD

#### Descrição
Expanda a API para consultar, atualizar e remover um livro pelo identificador. Use os códigos de status HTTP para comunicar o resultado de cada operação.

#### Requisitos
O programa concluído deve:

- Implementar `GET /books/{book_id}` para retornar um livro específico
- Implementar `PUT /books/{book_id}` para atualizar o título e o autor de um livro
- Implementar `DELETE /books/{book_id}` para remover um livro
- Retornar o status `404 Not Found` quando o identificador não corresponder a um livro existente
- Retornar um status de sucesso apropriado para cada operação, incluindo `201 Created` ao criar um livro


### 🛠️ Validar e testar a API

#### Descrição
Adicione uma forma de filtrar o catálogo e escreva testes automatizados para verificar os principais comportamentos da API.

#### Requisitos
O programa concluído deve:

- Permitir filtrar `GET /books` por título usando um parâmetro de consulta, como `GET /books?title=python`
- Validar os dados de entrada para que título e autor não sejam valores vazios
- Criar testes com o `TestClient` do FastAPI para os endpoints de listagem, criação, consulta e remoção
- Verificar nos testes os códigos de status e o conteúdo das respostas, incluindo o caso de livro não encontrado
- Manter os dados em memória; persistência em banco de dados e autenticação não fazem parte desta atividade
