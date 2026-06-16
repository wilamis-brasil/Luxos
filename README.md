# Luxos — Dashboard

Implementação para trabalho acadêmico FIAP de uma tela única do protótipo fintech **Luxos**: o **Dashboard** do
usuário. Construído com **HTML5 semântico**, **CSS** e **Tailwind CSS**, com foco em
coerência visual com o protótipo, responsividade mobile-first e código limpo.

Visualize o site em: [https://wilamis-brasil.github.io/Luxos/](https://wilamis-brasil.github.io/Luxos/)

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
└── README.md
```

## Tecnologias e decisões

- **Tailwind CSS (Play CDN v4)**.
- **Separação HTML/CSS**.
- **Mobile-first**.
- **Acessibilidade**.
