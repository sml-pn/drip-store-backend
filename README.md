# <h1 align="center">Drip Store API</h1>

<p align="center">
  <strong>API RESTful desenvolvida para ser o backend da aplicação de e-commerce Drip Store</strong>
</p>

<p align="center">
  <a href="#-tecnologias">Tecnologias</a>   |   
  <a href="#-funcionalidades">Funcionalidades</a>   |   
  <a href="#-endpoints">Endpoints</a>   |   
  <a href="#-como-executar">Como executar</a>   |   
  <a href="#-licença">Licença</a>
</p>

<p align="center">
  <img alt="License" src="https://img.shields.io/static/v1?label=license&message=MIT&color=49AA26&labelColor=000000">
</p>

## ✨ Tecnologias

- **Node.js** - Ambiente de execução JavaScript
- **Express.js** - Framework para construção de APIs
- **Sequelize** - ORM para bancos de dados relacionais
- **PostgreSQL** - Banco de dados relacional
- **Docker** - Plataforma de containerização
- **JWT** - Autenticação via tokens
- **Bcrypt.js** - Hash de senhas
- **Jest & Supertest** - Testes automatizados
- **CORS** - Middleware para acesso entre origens

## 💻 Projeto

API completa para e-commerce com:

- Gestão de usuários e autenticação
- CRUD de produtos e categorias
- Busca avançada com filtros
- Arquitetura escalável

## 🔥 Funcionalidades Principais

- ✅ Autenticação JWT segura
- ✅ CRUD completo de usuários e produtos
- ✅ Filtros avançados de busca
- ✅ Middleware de proteção de rotas
- ✅ Ambiente dockerizado

## 📡 Endpoints Principais

| Método | Endpoint                | Descrição                      | Auth |
|--------|-------------------------|--------------------------------|:----:|
| POST   | `/usuario`              | Cria novo usuário              | Não  |
| POST   | `/usuario/token`        | Login (gera token JWT)         | Não  |
| GET    | `/produto/pesquisa`     | Busca produtos com filtros     | Não  |

*Lista completa disponível no código*

## 🚀 Como Executar

**Pré-requisitos:**
- Node.js 16+
- Docker instalado

```bash
# Clone o repositório
git clone https://github.com/sml-pn/drip-store-backend.git

# Instale dependências
npm install

# Inicie o container do PostgreSQL
docker run --name drip-store-db -e POSTGRES_PASSWORD=docker -p 5432:5432 -d postgres

# Execute a API
npm run dev

A API estará disponível em http://localhost:3001

🧪 Testes

npm test
📄 Licença
MIT License - LICENSE

<p align="center"> Desenvolvido com ❤️ por <a href="https://github.com/sml-pn">Samuel Pena</a> </p> ```