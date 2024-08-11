Projeto Express API
<br>
Este projeto é uma API simples criada usando o framework Express.js para gerenciar uma lista de usuários. A API permite criar, listar, atualizar e deletar usuários. Cada usuário possui um identificador único (UUID), nome e idade.

Instalação
Clone o repositório:
bash
Copiar código
git clone <URL_DO_REPOSITORIO>
Navegue até o diretório do projeto:
bash
Copiar código
cd nome-do-projeto
Instale as dependências:
bash
Copiar código
npm install
Uso
Para iniciar o servidor, execute:

bash
Copiar código
node app.js
O servidor será iniciado na porta 3000.

Endpoints
Listar Usuários
GET /projects

Retorna a lista de todos os usuários cadastrados.

Criar Usuário
POST /projects

Cria um novo usuário.

Body:
json
Copiar código
{
  "name": "Nome do Usuário",
  "age": "Idade do Usuário"
}
Atualizar Usuário
PUT /projects/

Atualiza um usuário específico.

Params: id do usuário.
Body:
json
Copiar código
{
  "name": "Novo Nome",
  "age": "Nova Idade"
}
Deletar Usuário
DELETE /projects/

Deleta um usuário específico.

Params: id do usuário.
Middleware
checkUserId
Middleware que verifica se o usuário existe antes de atualizar ou deletar. Se o usuário não for encontrado, retorna um erro 404.

Tecnologias
Node.js
Express.js
UUID (para geração de identificadores únicos)
