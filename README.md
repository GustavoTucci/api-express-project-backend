# API de Data e Hora

API REST leve para consulta da data e hora atuais. Desenvolvida com Node.js e Express, com CORS habilitado para integração com o frontend publicado no Vercel.

| Ambiente | Endereço |
| --- | --- |
| Repositório | [github.com/GustavoTucci/api-express-project-backend](https://github.com/GustavoTucci/api-express-project-backend) |
| Produção | [api-express-project-backend.onrender.com](https://api-express-project-backend.onrender.com) |
| Frontend integrado | [api-express-project-frontend.vercel.app](https://api-express-project-frontend.vercel.app/) |

## Stack

- Node.js 18+
- Express 5
- CORS

## Início rápido

```bash
npm install
npm start
```

O servidor local será executado em `http://localhost:3000`.

## Endpoint

### `GET /`

Retorna a data e a hora formatadas para o padrão brasileiro:

```json
{
  "date": "26/08/2026, 22:00:00",
  "status": "API no Render funcionando!"
}
```

| Status | Significado |
| --- | --- |
| `200 OK` | Consulta realizada com sucesso |

Teste a API em produção pelo link: [Consultar data e hora](https://api-express-project-backend.onrender.com/).

## Configuração

O servidor utiliza `process.env.PORT`, fornecida automaticamente pelo Render. Em ambiente local, o valor padrão é `3000`.

## Deploy

Para publicar este repositório no Render, crie um **Web Service** e configure:

- **Runtime:** Node
- **Build Command:** `npm install`
- **Start Command:** `npm start`

O CORS está habilitado para permitir chamadas feitas por aplicações hospedadas em outro domínio.

## Estrutura

```text
backend/
├── api.js
├── package.json
├── package-lock.json
├── .gitignore
└── README.md
```

## Licença

Projeto desenvolvido para fins educacionais.
