🤖 API - Agentes Inteligentes
Este projeto demonstra a criação de uma API moderna e eficiente para suportar agentes inteligentes, utilizando tecnologias recentes, arquitetura modular e boas práticas de desenvolvimento.

🚀 Tecnologias
Node.js com TypeScript nativo (experimental strip types)

Fastify – Framework web rápido e eficiente

PostgreSQL com extensão pgvector para armazenamento e busca de vetores

Drizzle ORM – Operações de banco de dados com tipagem segura

Zod – Validação de schemas e dados

Docker – Containerização do banco de dados

Biome – Linting e formatação de código

🏗️ Arquitetura
O projeto foi desenvolvido com foco em modularidade e escalabilidade:

Separação clara entre rotas, schemas e conexão com o banco

Validação de schemas com Zod para maior segurança de tipos

ORM Drizzle para consultas e migrações tipadas

Variáveis de ambiente centralizadas para fácil configuração

⚙️ Setup e Configuração
Pré-requisitos
Node.js (versão com suporte a --experimental-strip-types)

Docker e Docker Compose

1️⃣ Clone o repositório
bash
Copy
Edit
git clone <url-do-repositorio>
cd server
2️⃣ Configure o banco de dados
bash
Copy
Edit
docker-compose up -d
3️⃣ Configure as variáveis de ambiente
Crie um arquivo .env na raiz do projeto:

env
Copy
Edit
PORT=3333
DATABASE_URL=postgresql://docker:docker@localhost:5432/agents
4️⃣ Instale as dependências
bash
Copy
Edit
npm install
5️⃣ Execute as migrações do banco
bash
Copy
Edit
npx drizzle-kit migrate
6️⃣ (Opcional) Popule o banco com dados de exemplo
bash
Copy
Edit
npm run db:seed
7️⃣ Execute o projeto
Modo desenvolvimento:

bash
Copy
Edit
npm run dev
Modo produção:

bash
Copy
Edit
npm start
📚 Scripts Disponíveis
npm run dev – Executa o servidor em modo de desenvolvimento com hot reload

npm start – Executa o servidor em modo de produção

npm run db:seed – Popula o banco com dados de exemplo

🌐 Endpoints
A API estará disponível em http://localhost:3333

Método Endpoint Descrição
GET /health Health check da aplicação
GET /rooms Lista as salas disponíveis
