# Requisitos do Sistema

## Objetivo

Este documento descreve todos os requisitos funcionais e não funcionais do FinanceHub.

Os requisitos definidos neste documento servirão como base para a modelagem do banco de dados, desenvolvimento do backend, frontend e testes do sistema.

---

# Requisitos Funcionais

## Módulo: Autenticação

### RF001 - Cadastro de Usuário

**Descrição**

O sistema deve permitir que um visitante realize seu cadastro.

**Ator**

Visitante

**Prioridade**

Alta

**Dependências**

Nenhuma

**Status**

🟡 Planejado

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

🟡 Planejado

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

🟡 Planejado

**Versão**

v0.1.0

---

## Módulo: Contas

### RF004 - Cadastrar Conta

...

### RF005 - Editar Conta

...

### RF006 - Excluir Conta

...

---

## Módulo: Categorias

### RF007 - Cadastrar Categoria

...

### RF008 - Editar Categoria

...

### RF009 - Excluir Categoria

...

---

## Módulo: Movimentações

### RF010 - Registrar Receita

...

### RF011 - Registrar Despesa

...

### RF012 - Registrar Transferência

...

---

## Módulo: Dashboard

### RF013 - Visualizar Dashboard

...

---

## Módulo: Relatórios

### RF014 - Relatório por Categoria

...

### RF015 - Relatório Mensal

...

---

# Requisitos Não Funcionais

### RNF001 - Responsividade

O sistema deverá ser responsivo para dispositivos móveis e desktops.

---

### RNF002 - Segurança

As senhas deverão ser armazenadas de forma criptografada.

---

### RNF003 - API REST

O backend deverá disponibilizar uma API REST.

---

### RNF004 - Banco de Dados

O sistema utilizará PostgreSQL.

---

### RNF005 - Autenticação

O sistema utilizará JWT para autenticação.

---

### RNF006 - Performance

As operações deverão responder em tempo adequado para garantir boa experiência ao usuário.

---

# Fora do Escopo do MVP

Nesta seção serão registradas funcionalidades planejadas para versões futuras.

Exemplos:

- Open Finance
- Aplicativo Mobile
- IA
- Integrações externas
