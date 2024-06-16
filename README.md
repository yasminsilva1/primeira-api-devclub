# Projeto de API - CRUD de Usuários

<p>Este projeto consiste na criação de uma API do zero, seguindo o tutorial do canal <a href="https://www.youtube.com/watch?v=PyrMT0GA3sE&t=42s" target="_blank">DevClub | Programação</a> no YouTube.
</p>

<p>A API foi desenvolvida utilizando Node.js com Express e se conecta a um banco de dados MongoDB utilizando o Prisma ORM. A API implementa um CRUD (Create, Read, Update, Delete) para gerenciar uma lista de usuários.</p>

## Requisitos

<p>Para executar este projeto, você precisará:</p>

- Instalar o <a href="https://nodejs.org/en" target="_blank">Node.js</a>;
- Criar uma conta gratuita no
  <a href="https://www.mongodb.com/" target="_blank">MongoDB Atlas</a>;
- Instalar a extensão
  <a href="https://www.thunderclient.com/" target="_blank">Thunder Client</a> em
  sua IDE - Através de sua interface baseada em GUI fica fácil testar as API's.

## Instalação

<h3>1. Clone o repositório:</h3>

```bash
git clone https://github.com/yasminsilva1/primeira-api-devclub.git
cd primeira-api-devclub
```

<h3>2. Instale as dependências:</h3>

```bash
npm install
```

<h3>3. Configure o primas:</h3>

```bash
npx prisma init
```

<p>Isso criará um arquivo <code>.env</code> na raiz do projeto e um diretório <code>prisma</code> com o arquivo <code>schema.prisma</code>. Configure o <code>schema.prisma</code> de acordo com suas necessidades.</p>

<h3>4. Configure o MongoDB:</h3>
<p>No arquivo <code>.env</code> na raiz do projeto, adicione a URL de conexão com o MongoDB:</p>

```bash
DATABASE_URL="mongodb+srv://<usuário>:<senha>@cluster0.mongodb.net/<database>?retryWrites=true&w=majority"
```

<h3>5. Execute as migrações do Prisma:</h3>

```bash
npx prisma db push
```

<h3>6. Inicie o servidor:</h3>

```bash
node --watch server.js
```

<h2>Uso</h2>
<p>A API fornece os seguintes endpoints para gerenciar a lista de usuários:</p>

- <code>GET /users</code>: Retorna a lista de usuários.
- <code>GET /users/</code>: Retorna um usuário específico.
- <code>POST /users</code>: Cria um novo usuário.
- <code>PUT /users/</code>: Atualiza um usuário existente.
- <code>DELETE /users/</code>: Exclui um usuário.

<h2>Estrutura do Projeto</h2>

```bash
├── node_modules
├── prisma
│   └── schema.prisma
├── .env
├── .gitignore
├── package-lock.json
├── package.json
├── README.md
└── server.js
```

<h2>Licença</h2>
<p>Este projeto é licenciado sob os termos da licença MIT.</p>
<hr>
