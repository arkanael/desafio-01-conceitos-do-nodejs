# 🏛 Desafio 01 - Conceitos do Node.js

Esse desafio é para por em prática e treinar o aprendizado inicial do node.js.

## 💻 Sobre o Projeto

Essa é uma aplicação para gerenciar tarefas (em inglês _todos_). 
Será permitida a criação de um usuário com `name` e `username`, bem como fazer o CRUD de *todos*:

### 🧪 Tecnologias

- NodeJs (https://nodejs.org/)
- Express (https://expressjs.com/)
- Uuidv4 (https://www.npmjs.com/package/uuidv4)

### 🛠 Features

- Criar um novo _todo_;
- Listar todos os _todos_;
- Alterar o `title` e `deadline` de um _todo_ existente;
- Marcar um _todo_ como feito;
- Excluir um _todo_;

### 💲 Dados do TODO:

id: 'uuid', // precisa ser um uuid
title: 'Nome da tarefa',
done: false,
deadline: new Date(deadline),
created_at: new Date()

### 🌉 Rotas utiizadas:

### POST `/users`

A rota deve receber `name`, e `username` dentro do corpo da requisição. Ao cadastrar um novo usuário, ele deve ser armazenado dentro de um objeto no seguinte formato:

#### PUT `/todos/:id`

A rota deve receber, pelo header da requisição, uma propriedade `username` contendo o username do usuário e receber as propriedades `title` e `deadline` dentro do corpo. É preciso alterar **apenas** o `title` e o `deadline` da tarefa que possua o `id` igual ao `id` presente nos parâmetros da rota.

#### POST `/todos`

A rota deve receber `title` e `deadline` dentro do corpo da requisição e, uma propriedade `username` contendo o username do usuário dentro do header da requisição. Ao criar um novo _todo_, ele deve ser armazenada dentro da lista `todos` do usuário que está criando essa tarefa. Cada tarefa deverá estar no seguinte formato: . Certifique-se que o ID seja um UUID.

#### POST `/users`

A rota deve receber `name`, e `username` dentro do corpo da requisição. Ao cadastrar um novo usuário, ele deve ser armazenado dentro de um objeto no seguinte formato:

#### PATCH `/todos/:id/done`

A rota deve receber, pelo header da requisição, uma propriedade `username` contendo o username do usuário e alterar a propriedade `done` para `true` no _todo_ que possuir um `id` igual ao `id` presente nos parâmetros da rota.

#### DELETE `/todos/:id`

A rota deve receber, pelo header da requisição, uma propriedade `username` contendo o username do usuário e excluir o _todo_ que possuir um `id` igual ao `id` presente nos parâmetros da rota.

### 🆎 Status Code:

- status(201) => Criado com Sucesso.
- status(400) => Não pode processar
- status(404) => Não encontrado

### 📚 Legendas dos verbos HTTP

- GET => Buscar uma informação
- POST => Inserir uma informação
- PUT => Alterar uma informação
- PATCH => Alterar uma informação específica
- DELETE => Deleta uma informação

### 🚀 Meus Contatos

<h4>LinkedIn: <a href="https://www.linkedin.com/in/lbandeira/">www.linkedin.com/in/lbandeira/</a></h4>
<h4>Facebook: <a href="https://www.facebook.com/luiz.guilherme.58367/">https://www.facebook.com/luiz.guilherme.58367/</a></h4>
<h4>E-mail: <a href="mailto://arkanael@gmailcom/">arkanael@gmail.com</a></h4>
<h4>Currículo: <a href="https://arkanael.github.io/curriculo/">https://arkanael.github.io/curriculo/</a></h4>
<h4 align=center>Desenvolvido por Luiz Guilherme Bandeira</h4>
