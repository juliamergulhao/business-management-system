# Sistema de Gestão Empresarial 🏢

Sistema web de **gestão empresarial e análise de processos**, desenvolvido para demonstrar a integração entre arquitetura empresarial, processos de negócio, estoque, vendas e gestão financeira.

[![LIVE DEMO](https://img.shields.io/badge/LIVE_DEMO-ACESSAR_APLICAÇÃO-14c9b5?style=for-the-badge)](https://juliamergulhao.github.io/sistema-gestao-empresarial/)
[![SOURCE CODE](https://img.shields.io/badge/SOURCE_CODE-GITHUB-181717?style=for-the-badge&logo=github)](https://github.com/juliamergulhao/sistema-gestao-empresarial)

O projeto combina a análise e modelagem de processos **AS-IS e TO-BE** com módulos funcionais de **Estoque, Vendas, Contas a Pagar e Contas a Receber**, permitindo visualizar como processos, dados e sistemas podem trabalhar de forma integrada.

A aplicação também demonstra a integração entre diferentes áreas do negócio, como a atualização automática do estoque após uma venda e a geração de contas a receber em operações realizadas a prazo.

---

## 🎯 Objetivo

## 🎯 Objetivo do projeto

O objetivo é representar um cenário empresarial no qual processos de negócio podem ser analisados, redesenhados e apoiados por sistemas integrados.

O projeto aborda duas perspectivas:

- **Arquitetura e processos:** análise do cenário atual, identificação de problemas e proposta de melhoria.
- **Gestão operacional:** demonstração da integração entre estoque, vendas e financeiro.

---

## 🏗️ Arquitetura Empresarial

A aplicação apresenta a análise de um processo de **onboarding de fornecedores**, permitindo comparar o funcionamento atual com uma proposta de processo futuro.

### AS-IS

Representa o processo atual.

O cenário analisado apresenta problemas como:

- Esperas entre áreas;
- Handoffs excessivos;
- Reenvio de documentos;
- Validações repetidas;
- Redigitação de informações;
- Dados distribuídos entre diferentes sistemas;
- Falta de regras claras para tratamento de exceções.

O processo possui um lead time aproximado de **25 dias**, embora o trabalho efetivo seja inferior a **4 horas**.

### TO-BE

Representa a proposta de processo futuro.

Entre as melhorias apresentadas estão:

- Portal único para entrada de informações;
- Reutilização de dados;
- Validações realizadas em paralelo;
- Aplicação de regras automáticas;
- Separação entre casos padrão e exceções;
- Fila específica para tratamento de exceções;
- Integração com ERP e gestão de identidade.

A proposta busca reduzir esperas, retrabalho e transferências desnecessárias entre áreas.

---

## ⚙️ Funcionalidades

### 📦 Gestão de Estoque

Permite:

- Cadastrar produtos;
- Definir categoria;
- Controlar quantidade disponível;
- Definir estoque mínimo;
- Registrar preço de venda;
- Identificar produtos com estoque baixo.

### 🛒 Vendas

Permite registrar vendas informando dados como:

- Cliente;
- Produto;
- Quantidade;
- Data;
- Forma de pagamento.

Ao registrar uma venda, a quantidade vendida é automaticamente descontada do estoque.

### 💸 Contas a Pagar

Permite controlar obrigações financeiras da empresa, incluindo:

- Descrição;
- Fornecedor;
- Valor;
- Data de vencimento;
- Situação do pagamento.

### 💰 Contas a Receber

Permite acompanhar valores que a empresa possui para receber.

Vendas realizadas a prazo podem gerar automaticamente um registro em **Contas a Receber**, demonstrando a integração entre o processo comercial e financeiro.

---

## 🔄 Integração entre os módulos

Uma das principais características do projeto é a comunicação entre diferentes áreas do sistema.

Exemplo:

Venda registrada
        ↓
Atualização do estoque
        ↓
Venda a prazo
        ↓
Geração de conta a receber

Essa integração demonstra como uma única operação pode produzir efeitos em diferentes processos empresariais.

---

## 📊 Indicadores

O sistema também trabalha com indicadores para acompanhamento dos processos e operações.

Entre eles:

- Lead time do processo;
- Taxa de retrabalho;
- Taxa de automação;
- Produtos cadastrados;
- Produtos com estoque baixo;
- Quantidade de vendas;
- Faturamento;
- Total a pagar;
- Total a receber.

---

## 🧩 Conceitos abordados

O projeto aplica conceitos relacionados a:

- Arquitetura Empresarial;
- Processos de negócio;
- BPMN;
- AS-IS;
- TO-BE;
- Eventos;
- Tarefas;
- Gateways;
- Pools e Lanes;
- Handoffs;
- Gargalos;
- Retrabalho;
- Automação;
- Tratamento de exceções;
- Indicadores de desempenho;
- Integração entre processos e sistemas.

---

## 💻 Tecnologias utilizadas

- HTML5
- CSS3
- JavaScript
- LocalStorage
- Git
- GitHub
- GitHub Pages

O projeto foi desenvolvido em um único arquivo `index.html`, contendo estrutura, estilização e lógica da aplicação.

---

## 💾 Persistência dos dados

Os registros da aplicação são armazenados no **LocalStorage do navegador**.

Isso permite manter os dados cadastrados ao atualizar ou fechar a página no mesmo navegador.

> O projeto não utiliza banco de dados ou backend. Por isso, os dados permanecem armazenados localmente no navegador utilizado.

---

## 📁 Estrutura do projeto

```text
sistema-gestao-empresarial/
│
└── index.html
