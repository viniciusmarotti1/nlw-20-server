# 🤖 API - Agentes Inteligentes

Este projeto demonstra a criação de uma API moderna e eficiente para suportar agentes inteligentes, utilizando tecnologias recentes, arquitetura modular e boas práticas de desenvolvimento.

---

## 🚀 Tecnologias

- **Node.js com TypeScript nativo** (experimental strip types)
- **Fastify** – Framework web rápido e eficiente
- **PostgreSQL** com extensão **pgvector** para armazenamento e busca de vetores
- **Drizzle ORM** – Operações de banco de dados com tipagem segura
- **Zod** – Validação de schemas e dados
- **Docker** – Containerização do banco de dados
- **Biome** – Linting e formatação de código

---

## 🏗️ Arquitetura

O projeto foi desenvolvido com foco em modularidade e escalabilidade:

- Separação clara entre rotas, schemas e conexão com o banco
- Validação de schemas com **Zod** para maior segurança de tipos
- ORM **Drizzle** para consultas e migrações tipadas
- Variáveis de ambiente centralizadas para fácil configuração

---

## ⚙️ Setup e Configuração

### Pré-requisitos

- Node.js (versão com suporte a `--experimental-strip-types`)
- Docker e Docker Compose
