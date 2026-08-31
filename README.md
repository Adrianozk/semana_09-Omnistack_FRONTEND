# AirCnC Frontend — Semana OmniStack 9

Interface web do projeto desenvolvido durante a Semana OmniStack 9, da Rocketseat. Esta parte da aplicação é utilizada por empresas para cadastrar espaços de trabalho e administrar solicitações de reserva.

> **Contexto:** projeto de estudo criado em 2019. As versões das dependências refletem a edição original do curso.

## Funcionalidades

- Entrada por e-mail
- Cadastro de espaços com imagem, tecnologias e valor da diária
- Dashboard com os espaços cadastrados
- Recebimento de solicitações em tempo real com Socket.IO
- Aprovação ou rejeição de reservas

## Tecnologias

- React
- React Router
- Axios
- Socket.IO Client
- Create React App
- Yarn

## Repositórios relacionados

- [Backend](https://github.com/Adrianozk/semana_09-Omnistack_BACKEND)
- [Aplicativo mobile](https://github.com/Adrianozk/semana_09-Omnistack_MOBILE)

## Como executar

1. Inicie o backend na porta `3333`.
2. Instale as dependências:

```bash
yarn install
```

3. Confirme o endereço da API em `src/services/api.js`:

```javascript
const api = axios.create({
    baseURL: 'http://localhost:3333',
})
```

4. Inicie a aplicação:

```bash
yarn start
```

A interface será aberta normalmente em `http://localhost:3000`.

## Páginas

| Rota | Finalidade |
| --- | --- |
| `/` | Entrada por e-mail |
| `/dashboard` | Lista de espaços e solicitações |
| `/new` | Cadastro de um novo espaço |

## Estrutura

```text
src/
├── assets/       # imagens e elementos visuais
├── pages/        # Login, Dashboard e cadastro
├── services/     # cliente HTTP
├── routes.js     # rotas da interface
└── App.js        # componente principal
```

## Observação sobre compatibilidade

O projeto utiliza React 16 e React Scripts 3. Por ser um registro histórico de curso, pode exigir uma versão de Node.js compatível com dependências de 2019.
