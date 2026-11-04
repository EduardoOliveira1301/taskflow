# TaskFlow

Gerenciador de tarefas desenvolvido na disciplina de Desenvolvimento Mobile, com
React, TypeScript, React Router, Axios e CrudCrud (API REST usada como backend
temporário).

## Funcionalidades

- Navegação entre as páginas Hoje, Próximas, Todas as tarefas e Concluídas (SPA).
- Carregamento das tarefas a partir do CrudCrud.
- Cadastro de tarefas por meio de um modal único, acessível pela Sidebar, pelo
  Header e pela página Todas as tarefas.
- Exclusão de tarefas.

## Requisitos

- Node.js 20 ou superior
- Um endpoint do [CrudCrud](https://crudcrud.com)

## Como executar

```bash
npm install
cp .env.example .env
```

Edite o arquivo `.env` e troque `SEU_ENDPOINT` pelo identificador gerado no
CrudCrud:

```env
VITE_API_URL=https://crudcrud.com/api/SEU_ENDPOINT
```

Depois, inicie o servidor de desenvolvimento:

```bash
npm run dev
```

> O endpoint gratuito do CrudCrud é temporário. Se as requisições começarem a
> falhar, gere um novo endpoint, atualize o `.env` e reinicie o `npm run dev`
> (o Vite só lê o `.env` ao iniciar).

## Scripts

| Comando           | Descrição                                   |
| ----------------- | ------------------------------------------- |
| `npm run dev`     | Inicia o servidor de desenvolvimento        |
| `npm run build`   | Verifica os tipos e gera a versão de produção |
| `npm run preview` | Executa localmente a versão de produção     |

## Estrutura

```text
src/
├── components/   Layout, Sidebar, Header, TaskCard, TaskList, TaskForm, TaskModal
├── contexts/     TarefasContext (estado compartilhado das tarefas)
├── pages/        Today, Upcoming, Tasks, Completed
├── services/     tarefaService (comunicação HTTP com o CrudCrud)
├── styles/       variables.css e global.css
└── types/        Tarefa
```
