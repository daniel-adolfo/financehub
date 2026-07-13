# Requisitos do Sistema

## Objetivo

Este documento descreve os requisitos funcionais e não funcionais do FinanceHub.

Os requisitos definidos aqui servirão como base para a modelagem do banco de dados, desenvolvimento do backend, frontend e testes da aplicação.

---

# Requisitos Funcionais

## Módulo: Autenticação

### RF001 – Cadastro de Usuário

| Campo | Valor |
|--------|-------|
| **Descrição** | O sistema deve permitir que um visitante realize seu cadastro informando nome, e-mail e senha. |
| **Ator** | Visitante |
| **Prioridade** | Alta |
| **Dependências** | Nenhuma |
| **Status** | 🟡 Planejado |
| **Versão** | v0.1.0 |

### RF002 – Login

| Campo | Valor |
|--------|-------|
| **Descrição** | O sistema deve permitir que o usuário realize login utilizando e-mail e senha. |
| **Ator** | Usuário |
| **Prioridade** | Alta |
| **Dependências** | RF001 |
| **Status** | 🟡 Planejado |
| **Versão** | v0.1.0 |

### RF003 – Logout

| Campo | Valor |
|--------|-------|
| **Descrição** | O sistema deve permitir que o usuário encerre sua sessão de forma segura. |
| **Ator** | Usuário |
| **Prioridade** | Alta |
| **Dependências** | RF002 |
| **Status** | 🟡 Planejado |
| **Versão** | v0.1.0 |

---

## Módulo: Contas

### RF004 – Cadastrar Conta

| Campo | Valor |
|--------|-------|
| **Descrição** | O sistema deve permitir que o usuário cadastre contas financeiras como bancos, carteiras ou contas digitais. |
| **Ator** | Usuário |
| **Prioridade** | Alta |
| **Dependências** | RF002 |
| **Status** | 🟡 Planejado |
| **Versão** | v0.1.0 |

### RF005 – Editar Conta

| Campo | Valor |
|--------|-------|
| **Descrição** | O sistema deve permitir alterar as informações de uma conta existente. |
| **Ator** | Usuário |
| **Prioridade** | Alta |
| **Dependências** | RF004 |
| **Status** | 🟡 Planejado |
| **Versão** | v0.1.0 |

### RF006 – Excluir Conta

| Campo | Valor |
|--------|-------|
| **Descrição** | O sistema deve permitir excluir uma conta que não possua movimentações associadas. |
| **Ator** | Usuário |
| **Prioridade** | Média |
| **Dependências** | RF004 |
| **Status** | 🟡 Planejado |
| **Versão** | v0.1.0 |

---

## Módulo: Categorias

### RF007 – Cadastrar Categoria

| Campo | Valor |
|--------|-------|
| **Descrição** | O sistema deve permitir criar categorias personalizadas para organizar movimentações financeiras. |
| **Ator** | Usuário |
| **Prioridade** | Alta |
| **Dependências** | RF002 |
| **Status** | 🟡 Planejado |
| **Versão** | v0.1.0 |

### RF008 – Editar Categoria

| Campo | Valor |
|--------|-------|
| **Descrição** | O sistema deve permitir editar categorias existentes. |
| **Ator** | Usuário |
| **Prioridade** | Média |
| **Dependências** | RF007 |
| **Status** | 🟡 Planejado |
| **Versão** | v0.1.0 |

### RF009 – Excluir Categoria

| Campo | Valor |
|--------|-------|
| **Descrição** | O sistema deve permitir excluir categorias que não possuam movimentações vinculadas. |
| **Ator** | Usuário |
| **Prioridade** | Média |
| **Dependências** | RF007 |
| **Status** | 🟡 Planejado |
| **Versão** | v0.1.0 |

---

## Módulo: Movimentações Financeiras

### RF010 – Registrar Movimentação Financeira

| Campo | Valor |
|--------|-------|
| **Descrição** | O sistema deve permitir registrar movimentações financeiras do tipo Receita, Despesa ou Transferência. |
| **Ator** | Usuário |
| **Prioridade** | Alta |
| **Dependências** | RF004, RF007 |
| **Status** | 🟡 Planejado |
| **Versão** | v0.1.0 |

### RF011 – Editar Movimentação Financeira

| Campo | Valor |
|--------|-------|
| **Descrição** | O sistema deve permitir editar uma movimentação financeira existente. |
| **Ator** | Usuário |
| **Prioridade** | Alta |
| **Dependências** | RF010 |
| **Status** | 🟡 Planejado |
| **Versão** | v0.1.0 |

### RF012 – Excluir Movimentação Financeira

| Campo | Valor |
|--------|-------|
| **Descrição** | O sistema deve permitir excluir uma movimentação financeira registrada. |
| **Ator** | Usuário |
| **Prioridade** | Média |
| **Dependências** | RF010 |
| **Status** | 🟡 Planejado |
| **Versão** | v0.1.0 |

---

## Módulo: Dashboard

### RF013 – Visualizar Dashboard

| Campo | Valor |
|--------|-------|
| **Descrição** | O sistema deve apresentar um painel contendo saldo, receitas, despesas, gráficos e indicadores financeiros. |
| **Ator** | Usuário |
| **Prioridade** | Alta |
| **Dependências** | RF010 |
| **Status** | 🟡 Planejado |
| **Versão** | v0.1.0 |

---

## Módulo: Relatórios

### RF014 – Relatório por Categoria

| Campo | Valor |
|--------|-------|
| **Descrição** | O sistema deve permitir visualizar relatórios de movimentações agrupadas por categoria. |
| **Ator** | Usuário |
| **Prioridade** | Média |
| **Dependências** | RF010 |
| **Status** | 🟡 Planejado |
| **Versão** | v0.1.0 |

### RF015 – Relatório Mensal

| Campo | Valor |
|--------|-------|
| **Descrição** | O sistema deve permitir visualizar relatórios mensais de receitas e despesas. |
| **Ator** | Usuário |
| **Prioridade** | Média |
| **Dependências** | RF010 |
| **Status** | 🟡 Planejado |
| **Versão** | v0.1.0 |

---

# Requisitos Não Funcionais

| Código | Descrição |
|--------|-----------|
| RNF001 | O sistema deverá possuir interface responsiva para dispositivos móveis e desktops. |
| RNF002 | As senhas deverão ser armazenadas de forma criptografada. |
| RNF003 | O backend deverá disponibilizar uma API REST. |
| RNF004 | O banco de dados utilizado será PostgreSQL. |
| RNF005 | O sistema utilizará autenticação baseada em JWT. |
| RNF006 | O sistema deverá apresentar bom desempenho para operações comuns de consulta e cadastro. |

---

# Fora do Escopo do MVP

As funcionalidades abaixo estão previstas para versões futuras:

- Cartões de crédito
- Parcelamentos
- Metas financeiras
- Orçamentos
- Contas recorrentes
- Notificações
- Exportação para PDF
- Exportação para Excel
- Aplicativo Mobile
- Inteligência Artificial
- Integração com Open Finance
