# API de Data e Hora

API REST desenvolvida com Node.js e Express para disponibilizar a data e a hora atuais em formato JSON. O serviço possui suporte a CORS e está preparado para execução local ou hospedagem no Render.

## Tecnologias

- Node.js
- Express 5
- CORS

## Pré-requisitos

- Node.js 18 ou superior
- npm

## Instalação e execução

Clone o repositório, acesse a pasta do projeto e instale as dependências:

```bash
npm install
npm start
```

Por padrão, o servidor será iniciado em `http://localhost:3000`.

## API

### Consultar data e hora

`GET /`

Exemplo de resposta:

```json
{
  "date": "26/08/2026, 22:00:00",
  "status": "API no Render funcionando!"
}
```

### Códigos de resposta

| Código | Descrição |
| --- | --- |
| `200` | Consulta realizada com sucesso |

## Configuração

O servidor utiliza a variável de ambiente `PORT`. Quando ela não está definida, a porta `3000` é utilizada automaticamente.

## Deploy no Render

1. Crie um novo **Web Service** no Render.
2. Conecte o repositório deste backend.
3. Configure o ambiente como **Node**.
4. Use `npm install` em **Build Command**.
5. Use `npm start` em **Start Command**.
6. Confirme a criação do serviço.

O Render define a variável `PORT` automaticamente. Após a publicação, a API estará disponível em uma URL semelhante a:

```text
https://seu-backend.onrender.com/
```

## Estrutura

```text
backend/
├── api.js
├── package.json
├── package-lock.json
└── README.md
```

## Licença

Projeto desenvolvido para fins educacionais.
