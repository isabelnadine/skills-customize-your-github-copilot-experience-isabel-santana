# 📘 Atividade: Persistência de Dados com SQLite e FastAPI

## 🎯 Objetivo

Amplie a API de livros criada anteriormente para armazenar os dados em um banco SQLite, em vez de mantê-los apenas na memória. Você praticará a criação de tabelas, consultas SQL e testes que verificam a persistência dos dados.

## 📝 Tarefas

### 🛠️ Criar o banco de dados e a tabela de livros

#### Descrição
Configure o acesso a um banco SQLite para a API e crie a tabela que armazenará os livros. Use o módulo `sqlite3` da biblioteca padrão do Python.

#### Requisitos
O programa concluído deve:

- Criar ou abrir um arquivo de banco de dados SQLite ao iniciar a aplicação
- Criar uma tabela `books` com identificador, título e autor
- Definir o identificador como chave primária e exigir título e autor
- Poder iniciar mais de uma vez sem falhar quando a tabela já existir

### 🛠️ Salvar e listar livros no SQLite

#### Descrição
Substitua o armazenamento em memória dos endpoints de criação e listagem por operações no banco de dados. Mantenha o formato das respostas da API anterior.

#### Requisitos
O programa concluído deve:

- Salvar um livro enviado a `POST /books` na tabela `books`
- Retornar o livro criado e seu identificador, mantendo o status `201 Created`
- Retornar os livros armazenados em `GET /books`
- Usar consultas SQL parametrizadas ao inserir e consultar dados
- Continuar exibindo os livros depois que a aplicação for encerrada e iniciada novamente

### 🛠️ Completar o CRUD e testar a persistência

#### Descrição
Atualize os endpoints de consulta, edição e remoção para usar o SQLite e escreva testes automatizados para verificar o comportamento da API com um banco de teste separado.

#### Requisitos
O programa concluído deve:

- Implementar `GET /books/{book_id}`, `PUT /books/{book_id}` e `DELETE /books/{book_id}` usando o banco de dados
- Retornar `404 Not Found` quando o livro solicitado não existir
- Usar um banco de dados temporário ou separado nos testes para não alterar os dados de desenvolvimento
- Testar a criação e a consulta de um livro, a atualização e remoção e o caso de identificador inexistente
- Confirmar que um livro criado continua disponível após abrir uma nova conexão com o banco de dados
