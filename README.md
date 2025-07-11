# NLW Agents

Este projeto foi desenvolvido durante o evento **NLW (Next Level Week)** da Rocketseat. Ele é uma aplicação backend que utiliza tecnologias modernas e segue boas práticas de desenvolvimento.

## 🚀 Tecnologias utilizadas

- **Node.js**
- **TypeScript**
- **Express**
- **Drizzle ORM**
- **PostgreSQL**
- **Zod** (validações)
- **Dotenv** (variáveis de ambiente)
- **ESLint + Biome** (padronização de código)
- **Docker** (ambiente de banco de dados)
- **Vite** (caso tenha interface frontend acoplada - não confirmado)
- **PNPM** (gerenciador de pacotes)

## 🧱 Padrões e Estrutura

- **Camada de rotas separada**
- **Validação com Zod**
- **ORM com Drizzle**
- **Arquitetura modular (ex: `routes/`, `schemas/`, `lib/`)**
- **Variáveis de ambiente em `.env` e `.env.example`**
- **Scripts no `package.json` para facilitar o desenvolvimento**

## ⚙️ Como rodar o projeto

### Pré-requisitos

- Node.js 18+
- PNPM
- Docker (para o banco de dados)

### Instalação

## 🛢 Banco de Dados

```bash
# Inicie o banco com Docker
docker-compose up -d
```
## 🔃 Migrações

```bash
# Rodar as migrações com Drizzle
pnpm drizzle:push
```

## 🧪 Servidor de Desenvolvimento

```bash
# Rodar o servidor em modo desenvolvimento
pnpm dev
```
## 📁 Scripts úteis

```bash
pnpm dev             # Inicia o servidor com recarregamento automático
pnpm format          # Formata o código com Biome
pnpm lint            # Checa problemas de lint
pnpm drizzle:push    # Aplica migrações do banco
pnpm drizzle:studio  # Visualiza o banco com Drizzle Studio
