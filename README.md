Minha API TypeScript
Esta é uma API TypeScript simples que lida com usuários e tarefas. A API tem endpoints para criar, atualizar, excluir e listar usuários e tarefas. Ele também tem endpoints para adicionar tarefas a usuários específicos e para listar todas as tarefas de um usuário específico.

Tecnologias utilizadas
TypeScript
Node.js
Express
MongoDB
Mongoose
Configuração
Clone este repositório para sua máquina local
Certifique-se de ter o Node.js instalado em sua máquina
Instale as dependências executando npm install na pasta raiz do projeto
Configure as variáveis de ambiente em um arquivo .env. O exemplo do arquivo .env.example está disponível na raiz do projeto.
Inicie o servidor executando npm start
Endpoints
Usuários
GET /users - lista todos os usuários
GET /users/:id - lista um usuário pelo ID
POST /users - cria um novo usuário
PUT /users/:id - atualiza um usuário existente
DELETE /users/:id - exclui um usuário existente
Tarefas
GET /tasks - lista todas as tarefas
GET /tasks/:id - lista uma tarefa pelo ID
POST /tasks - cria uma nova tarefa
PUT /tasks/:id - atualiza uma tarefa existente
DELETE /tasks/:id - exclui uma tarefa existente
GET /users/:userId/tasks - lista todas as tarefas de um usuário
POST /users/:userId/tasks - adiciona uma nova tarefa a um usuário
Exemplo de solicitação
Criar um usuário:

bash
Copy code
POST /users
Content-Type: application/json

{
    "name": "João",
    "email": "joao@email.com",
    "password": "123456"
}
Resposta:

makefile
Copy code
Status: 201 Created
Content-Type: application/json

{
    "_id": "60ac7c17e796bf2c7e13d343",
    "name": "João",
    "email": "joao@email.com",
    "password": "123456",
    "__v": 0
}
Autor
Seu nome aqui

Licença
Este projeto está licenciado sob a Licença MIT - consulte o arquivo LICENSE.md para obter detalhes.
