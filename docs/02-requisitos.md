# Requisitos do Sistema

## 1. Introdução

### 1.1 Objetivo

Este documento tem como objetivo especificar os requisitos funcionais e não funcionais do **FinanceHub**, um sistema web para gerenciamento financeiro pessoal. A documentação servirá como referência para o desenvolvimento, testes e manutenção da aplicação, garantindo que todas as funcionalidades sejam implementadas de forma consistente e alinhadas aos objetivos do projeto.

### 1.2 Escopo

O FinanceHub é uma aplicação web desenvolvida para auxiliar usuários no controle de suas finanças pessoais. O sistema permitirá registrar receitas, despesas, contas bancárias, cartões de crédito, categorias e metas financeiras, além de disponibilizar dashboards e relatórios que facilitem o acompanhamento da situação financeira.

O sistema contará com autenticação de usuários, garantindo que cada pessoa tenha acesso apenas às suas próprias informações. A aplicação será desenvolvida utilizando uma arquitetura moderna, com backend em Spring Boot, frontend em React e banco de dados MySQL.

### 1.3 Definições

| Termo           | Definição                                                                                  |
| --------------- | ------------------------------------------------------------------------------------------ |
| Usuário         | Pessoa cadastrada no sistema que utiliza o FinanceHub para controlar suas finanças.        |
| Receita         | Qualquer entrada de dinheiro registrada pelo usuário.                                      |
| Despesa         | Qualquer saída de dinheiro registrada pelo usuário.                                        |
| Categoria       | Classificação utilizada para organizar receitas e despesas.                                |
| Conta           | Conta bancária, carteira ou outra origem de saldo financeiro.                              |
| Cartão          | Cartão de crédito utilizado para registrar compras e controlar faturas.                    |
| Meta Financeira | Objetivo financeiro definido pelo usuário, como economizar ou investir determinado valor.  |
| Dashboard       | Painel inicial com indicadores, gráficos e resumo da situação financeira.                  |
| Relatório       | Documento ou visualização que apresenta informações financeiras consolidadas para análise. |

## 2. Requisitos Funcionais

### RF01 – Cadastro de Usuários

**Descrição**

O sistema deverá permitir que novos usuários realizem seu cadastro para utilizar o FinanceHub.

**Entradas**

* Nome completo
* E-mail
* Senha
* Confirmação da senha

**Regras**

* O e-mail deverá ser único.
* A senha deverá atender aos critérios mínimos de segurança.
* A confirmação da senha deverá ser igual à senha informada.

**Saídas**

* Cadastro realizado com sucesso.
* Mensagem de erro caso exista alguma inconsistência nos dados informados.

**Prioridade**

Alta

---

### RF02 – Autenticação de Usuários

**Descrição**

O sistema deverá permitir que usuários cadastrados realizem login para acessar suas informações financeiras.

**Entradas**

* E-mail
* Senha

**Regras**

* Apenas usuários cadastrados poderão acessar o sistema.
* As credenciais deverão ser validadas antes da autenticação.
* O acesso às funcionalidades protegidas exigirá autenticação.

**Saídas**

* Login realizado com sucesso.
* Mensagem de erro para credenciais inválidas.
* Encerramento da sessão por meio da funcionalidade de logout.

**Prioridade**

Alta

---

### RF03 – Dashboard Financeiro

**Descrição**

O sistema deverá apresentar um painel inicial com um resumo da situação financeira do usuário.

**Informações exibidas**

* Saldo total.
* Total de receitas.
* Total de despesas.
* Saldo do mês.
* Últimas movimentações.
* Gráficos financeiros.
* Resumo por categorias.

**Regras**

* As informações deverão considerar apenas os dados do usuário autenticado.
* Os valores deverão ser atualizados automaticamente após qualquer movimentação financeira.

**Prioridade**

Alta
