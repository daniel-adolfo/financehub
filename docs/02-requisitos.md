# Requisitos do Sistema

## Objetivo

Este documento descreve os requisitos funcionais e não funcionais do FinanceHub.

Os requisitos definidos servirão como base para a modelagem do banco de dados, desenvolvimento do backend, frontend e testes do sistema.

---

# Requisitos Funcionais

## Módulo: Autenticação

### RF001 - Cadastro de Usuário

**Descrição**

O sistema deve permitir que um visitante realize seu cadastro informando nome, e-mail e senha.

**Ator**

Visitante

**Prioridade**

Alta

**Dependências**

Nenhuma

**Status**

Planejado

**Versão**

v0.1.0

---

### RF002 - Login

**Descrição**

O sistema deve permitir que o usuário realize login utilizando e-mail e senha.

**Ator**

Usuário

**Prioridade**

Alta

**Dependências**

RF001

**Status**

Planejado

**Versão**

v0.1.0

---

### RF003 - Logout

**Descrição**

O sistema deve permitir que o usuário encerre sua sessão.

**Ator**

Usuário

**Prioridade**

Alta

**Dependências**

RF002

**Status**

Planejado

**Versão**

v0.1.0

---

## Módulo: Contas

### RF004 - Cadastrar Conta

**Descrição**

O sistema deve permitir cadastrar contas financeiras.

**Ator**

Usuário

**Prioridade**

Alta

**Dependências**

RF002

**Status**

Planejado

**Versão**

v0.1.0

---

### RF005 - Editar Conta

**Descrição**

O sistema deve permitir editar contas cadastradas.

**Ator**

Usuário

**Prioridade**

Alta

**Dependências**

RF004

**Status**

Planejado

**Versão**

v0.1.0

---

### RF006 - Excluir Conta

**Descrição**

O sistema deve permitir excluir contas sem movimentações associadas.

**Ator**

Usuário

**Prioridade**

Média

**Dependências**

RF004

**Status**

Planejado

**Versão**

v0.1.0

---

## Módulo: Categorias

### RF007 - Cadastrar Categoria

**Descrição**

O sistema deve permitir criar categorias para organizar movimentações financeiras.

**Ator**

Usuário

**Prioridade**

Alta

**Dependências**

RF002

**Status**

Planejado

**Versão**

v0.1.0

---

## Módulo: Movimentações Financeiras

### RF008 - Registrar Movimentação Financeira

**Descrição**

O sistema deve permitir registrar movimentações do tipo Receita, Despesa e Transferência.

**Ator**

Usuário

**Prioridade**

Alta

**Dependências**

RF004 e RF007

**Status**

Planejado

**Versão**

v0.1.0

---

### RF009 - Editar Movimentação Financeira

**Descrição**

O sistema deve permitir editar movimentações financeiras.

**Ator**

Usuário

**Prioridade**

Alta

**Dependências**

RF008

**Status**

Planejado

**Versão**

v0.1.0

---

### RF010 - Excluir Movimentação Financeira

**Descrição**

O sistema deve permitir excluir movimentações financeiras.

**Ator**

Usuário

**Prioridade**

Média

**Dependências**

RF008

**Status**

Planejado

**Versão**

v0.1.0

---

## Módulo: Dashboard

### RF011 - Visualizar Dashboard

**Descrição**

O sistema deve apresentar um painel contendo saldo, receitas, despesas, gráficos e indicadores financeiros.

**Ator**

Usuário

**Prioridade**

Alta

**Dependências**

RF008

**Status**

Planejado

**Versão**

v0.1.0

---

## Módulo: Relatórios

### RF012 - Relatório por Categoria

**Descrição**

O sistema deve permitir visualizar movimentações agrupadas por categoria.

**Ator**

Usuário

**Prioridade**

Média

**Dependências**

RF008

**Status**

Planejado

**Versão**

v0.1.0

---

### RF013 - Relatório Mensal

**Descrição**

O sistema deve permitir visualizar relatórios mensais de receitas e despesas.

**Ator**

Usuário

**Prioridade**

Média

**Dependências**

RF008

**Status**

Planejado

**Versão**

v0.1.0

---

# Requisitos Não Funcionais

### RNF001

O sistema deverá possuir interface responsiva.

---

### RNF002

As senhas deverão ser armazenadas utilizando criptografia.

---

### RNF003

O backend deverá ser desenvolvido utilizando Java e Spring Boot.

---

### RNF004

O banco de dados será PostgreSQL.

---

### RNF005

O sistema utilizará autenticação baseada em JWT.

---

### RNF006

O sistema deverá possuir arquitetura REST.

---

# Fora do Escopo do MVP

As funcionalidades abaixo serão implementadas em versões futuras:

- Cartões de crédito.
- Parcelamentos.
- Metas financeiras.
- Orçamentos.
- Contas recorrentes.
- Exportação de relatórios.
- Aplicativo mobile.
- Inteligência Artificial.
- Integração com Open Finance.
