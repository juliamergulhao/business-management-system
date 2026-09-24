# Sistema de Gestão Empresarial 🏢

Sistema web para **gestão empresarial e análise de processos de negócio**, integrando modelagem de processos, estoque, vendas e controle financeiro em uma única aplicação.

[![Live Demo](https://img.shields.io/badge/Live%20Demo-Acessar%20Aplicação-00C7B7?style=for-the-badge)](https://juliamergulhao.github.io/sistema-gestao-empresarial/)
[![GitHub](https://img.shields.io/badge/Source%20Code-GitHub-181717?style=for-the-badge&logo=github)](https://github.com/juliamergulhao/sistema-gestao-empresarial)

O projeto combina conceitos de **Arquitetura Empresarial e processos de negócio** com módulos funcionais de **Estoque, Vendas, Contas a Pagar e Contas a Receber**.

A aplicação também apresenta a análise do processo de onboarding de fornecedores, comparando o cenário atual (**AS-IS**) com uma proposta de melhoria (**TO-BE**).

---

## 🎯 Objetivo

Demonstrar como **processos, dados, áreas de negócio e sistemas** podem funcionar de forma integrada dentro de uma organização.

A solução permite trabalhar com:

- Modelagem do processo atual (AS-IS)
- Modelagem do processo futuro (TO-BE)
- Identificação de gargalos e retrabalho
- Análise de handoffs entre áreas
- Indicadores de processo
- Gestão de estoque
- Registro de vendas
- Controle de contas a pagar
- Controle de contas a receber
- Integração entre operações comerciais e financeiras

---

## ⚙️ Funcionalidades

### 📊 Dashboard

- Visão consolidada da operação
- Produtos cadastrados
- Produtos com estoque baixo
- Quantidade de vendas
- Faturamento
- Valores a receber
- Valores a pagar

### 🏗️ Arquitetura e Processos

- Visualização do fluxo AS-IS
- Visualização do fluxo TO-BE
- Conceitos de processos de negócio
- Descrição dos procedimentos
- Identificação de gargalos
- Identificação de retrabalho
- Análise de handoffs
- Tratamento de exceções
- Indicadores de desempenho
- Justificativas para as melhorias propostas

### 📦 Estoque

- Cadastro de produtos
- Controle de quantidade
- Definição de estoque mínimo
- Cadastro de categoria
- Definição de preço de venda
- Identificação de produtos com estoque baixo
- Atualização automática após uma venda

### 🛒 Vendas

- Registro de vendas
- Seleção de produtos
- Identificação do cliente
- Controle de quantidade
- Registro da forma de pagamento
- Cálculo do valor da venda
- Baixa automática no estoque

### 💸 Contas a Pagar

- Cadastro de despesas
- Identificação do fornecedor
- Controle de valores
- Controle de vencimentos
- Acompanhamento da situação do pagamento

### 💰 Contas a Receber

- Cadastro de recebíveis
- Identificação do cliente
- Controle de valores
- Controle de vencimentos
- Integração com vendas realizadas a prazo

---

## 🔄 Integração dos Processos

A aplicação demonstra como uma operação pode gerar efeitos em diferentes áreas do negócio.

```text
Venda registrada
       │
       ▼
Atualização do estoque
       │
       ▼
Forma de pagamento
       │
       ├── À vista ──► Venda concluída
       │
       └── A prazo
              │
              ▼
       Conta a Receber
