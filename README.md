<h1 align="center">UserAPI 👥🤖</h1>


API CRUD com Express

<p align="center">
    Este projeto é uma API REST que usa o framework Express em Node.js e realiza operações CRUD para gerenciar usuários. É útil para entender como construir uma API básica e gerenciar recursos.</p>

---

## 📖 Sobre o projeto

Esse projeto é um exemplo de uma API REST simples construída com o framework Express em Node.js. A API fornece uma maneira de gerenciar usuários por meio das operações CRUD (Create, Read, Update e Delete).

Os usuários são armazenados em memória e são gerados identificadores exclusivos usando a biblioteca uuid. A API usa JSON como formato de dados para comunicação com o cliente.

O projeto é útil para entender como construir uma API REST básica usando o Express e como realizar operações CRUD para gerenciar recursos. Além disso, ele também demonstra como usar a biblioteca uuid para gerar identificadores exclusivos e como formatar os dados usando JSON.


## 🛠️ Tecnologias utilizadas

- Java Script
- NodeJS
- Visual Studio Code
- Insomnia

## Dependências

🤖 Este projeto foi desenvolvido utilizando as seguintes dependências:

- Express: ^4.17.1
- uuid: ^8.3.2

## Como executar 🚀

1. Instale as dependências do projeto com o comando:

<pre class="command">
`npm install`
</pre>


2. Inicie o servidor com o comando:

<pre class="command">
`npm start`
</pre>


O servidor estará disponível em `http://localhost:3000`.

## Rotas e requisições

A API possui as seguintes rotas e requisições:

### `GET /users`

Retorna todos os usuários cadastrados.

Exemplo de resposta:

```
[
{
"id": "2fa4c4a4-2a56-4c70-b1a5-1d7e6153d9ac",
"name": "Alice",
"age": 25
},
{
"id": "44ce6df9-6b1c-4a70-b95d-cf131d97f631",
"name": "Bob",
"age": 30
}
]
```


### `POST /users`

Cria um novo usuário.

Exemplo de requisição:

POST /users
Content-Type: application/json
```
{
"name": "Charlie",
"age": 40
}
```


Exemplo de resposta:

```
{
"id": "8a4fa966-48a2-4eaf-a7c8-51a77cc290fb",
"name": "Charlie",
"age": 40
}
```

### `PUT /users/:id`

Atualiza os dados de um usuário existente.

Exemplo de requisição:

PUT /users/2fa4c4a4-2a56-4c70-b1a5-1d7e6153d9ac
Content-Type: application/json
```
{
"name": "Alice Silva",
"age": 26
}
```

Exemplo de resposta:
```
[
{
"id": "2fa4c4a4-2a56-4c70-b1a5-1d7e6153d9ac",
"name": "Alice Silva",
"age": 26
},
{
"id": "44ce6df9-6b1c-4a70-b95d-cf131d97f631",
"name": "Bob",
"age": 30
}
]
```


### `DELETE /users/:id`

Remove um usuário existente.

Exemplo de requisição:

DELETE /users/2fa4c4a4-2a56-4c70-b1a5-1d7e6153d9ac


Exemplo de resposta:

204 No Content


## Testando as rotas com o Insomnia

O Insomnia é uma ferramenta que permite testar as rotas de uma API. Para testar as rotas desta API, faça o seguinte:

1. Instale o Insomnia, seguindo as instruções do site https://insomnia.rest/download.

2. Abra o Insomnia e clique no botão "Import/Export".

3. Clique no botão "Import Data" e selecione a opção "From Clipboard".

4. Copie e cole o conteúdo do arquivo


## 🙋 Como contribuir

1. Clone o repositório
2. Crie uma branch (`git checkout -b feature/sua-feature`)
3. Commit suas mudanças (`git commit -m 'Adiciona uma nova feature'`)
4. Push para a branch (`git push origin feature/sua-feature`)
5. Abra um Pull Request


Feito com ❤️ e desenvolvido no Visual Studio Code.


