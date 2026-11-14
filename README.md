# Easy Doc — Web

Front-end do **Easy Doc**, plataforma que conecta **médicos** e **hospitais**: hospitais publicam plantões e médicos encontram e aceitam propostas de acordo com a sua especialidade.

Projeto de Extensão da disciplina *Programação Orientada a Objetos em Java* (2023.2) — Universidade Estácio de Sá.

> O back-end está em [easy-doc-api](https://github.com/gabrielfins/easy-doc-api).

## Funcionalidades

- Cadastro e login separados para **médicos** e **hospitais**
- Hospitais criam propostas de plantão (data e hora de início)
- Médicos consultam as propostas disponíveis
- Dashboard e calendário para cada perfil

## Tecnologias

- Angular
- TypeScript
- SCSS
- RxJS

## Estrutura

```
src/app/
├── components/        # Componentes reutilizáveis (button, ...)
├── pages/
│   ├── doctor/        # login, cadastro, dashboard e calendário do médico
│   └── hospital/      # login, cadastro, dashboard, calendário e criação de plantão
└── app.routes.ts      # Rotas
```

## Como executar

Pré-requisitos: Node.js e npm, e a [API](https://github.com/gabrielfins/easy-doc-api) rodando.

```bash
npm install
npm start
```

Acesse `http://localhost:4200`.

A URL da API é definida em `src/environments/environment.development.ts` (por padrão `http://localhost:8000/api`).

## Scripts

| Comando | Descrição |
| --- | --- |
| `npm start` | Servidor de desenvolvimento (`ng serve`) |
| `npm run build` | Build de produção em `dist/` |
| `npm test` | Testes unitários (Karma) |
