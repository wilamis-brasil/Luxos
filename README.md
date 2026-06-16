# Luxos — Dashboard

Implementação de uma tela única do protótipo fintech **Luxos**: o **Dashboard** do
usuário. Construído com **HTML5 semântico**, **CSS** e **Tailwind CSS**, com foco em
coerência visual com o protótipo, responsividade mobile-first e código limpo.

## Tela implementada

Dashboard com:

- **Sidebar de navegação** (vira topbar com menu hambúrguer no mobile);
- **Cards de resumo** — saldo disponível, receitas, despesas e reserva;
- **Ações rápidas** — transferir, pagar boleto, adicionar saldo, cartão;
- **Alertas** com selos de status (Urgente / Ok / Atenção);
- **Tabela de movimentações recentes** com cores e badges por status.

## Estrutura

```
Luxos/
├── index.html   # marcação semântica + classes utilitárias do Tailwind
├── styles.css   # CSS custom (fonte, fundo, foco acessível, scrollbar)
├── README.md
└── docs/         # protótipo (PDF) e análise de requisitos
```

## Como executar

Não há build: basta abrir `index.html` no navegador (o Tailwind é carregado via
Play CDN). Para servir localmente, opcionalmente:

```bash
python -m http.server 8000
# acesse http://localhost:8000
```

## Tecnologias e decisões

- **Tailwind CSS (Play CDN v4)** para estilização utilitária; cor da marca (`#14385f`)
  registrada como token `@theme` (`bg-brand`, `text-brand`).
- **Separação HTML/CSS**: nenhum estilo inline em elementos; customizações em `styles.css`.
- **Mobile-first**: estilos base para celular e breakpoints `sm:`/`lg:` para telas maiores.
- **Acessibilidade**: landmarks (`<aside>`, `<nav>`, `<header>`, `<main>`, `<section>`,
  `<footer>`), tabela semântica com `scope`, foco visível e menu mobile com `aria-expanded`.

## Versionamento (Git)

O repositório já está iniciado localmente. Para publicar em um repositório público:

```bash
git add .
git commit -m "feat: tela Dashboard do projeto Luxos"
git remote add origin <URL_DO_REPO>
git push -u origin main
```
