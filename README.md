# Fluxo de Tarefas

Projeto desenvolvido para a disciplina de Desenvolvimento Mobile. O Fluxo de Tarefas é uma aplicação web para organizar atividades do dia a dia, permitindo visualizar, cadastrar e excluir tarefas.

O projeto foi desenvolvido utilizando React, TypeScript e outras ferramentas do ecossistema JavaScript.

## Funcionalidades

- Visualizar as tarefas do dia.
- Consultar as próximas tarefas.
- Visualizar todas as tarefas cadastradas.
- Consultar tarefas concluídas.
- Adicionar novas tarefas por meio de um formulário em modal.
- Excluir tarefas.

## Tecnologias utilizadas

- React
- TypeScript
- Vite
- React Router
- Axios
- CrudCrud (API utilizada para armazenar as tarefas)

## Requisitos

- Node.js 20 ou superior.
- Endpoint ativo no [CrudCrud](https://crudcrud.com/).

## Como executar o projeto

1. Instale as dependências:

```bash
npm install
```

2. Crie o arquivo `.env` a partir do exemplo:

```bash
cp .env.example .env
```

No Windows PowerShell, também é possível usar:

```powershell
Copy-Item .env.example .env
```

3. Abra o arquivo `.env` e informe seu endpoint:

```env
VITE_API_URL=https://crudcrud.com/api/SEU_ENDPOINT
```

4. Inicie o projeto:

```bash
npm run dev
```

## Scripts disponíveis

| Comando | Descrição |
|---|---|
| `npm run dev` | Inicia o servidor de desenvolvimento. |
| `npm run build` | Verifica os tipos e gera a versão de produção. |
| `npm run preview` | Executa localmente a versão de produção. |

## Organização do projeto

```text
src/
├── components/
├── contexts/
├── pages/
├── services/
├── styles/
└── types/
```

Cada pasta reúne os arquivos de uma parte da aplicação, como componentes, páginas, estilos e serviços.
