# Sistema de Gestão Empresarial 🏢

Sistema web para **gestão empresarial e análise de processos de negócio**, integrando modelagem de processos, estoque, vendas e controle financeiro em uma única aplicação.

[![Live Demo](https://img.shields.io/badge/Live%20Demo-Acessar%20Aplicação-00C7B7?style=for-the-badge)](https://juliamergulhao.github.io/sistema-gestao-empresarial/)
[![GitHub](https://img.shields.io/badge/Source%20Code-GitHub-181717?style=for-the-badge&logo=github)](https://github.com/juliamergulhao/sistema-gestao-empresarial)

Projeto desenvolvido para demonstrar, de forma prática, a aplicação de conceitos de **Arquitetura Empresarial, processos de negócio e integração entre áreas operacionais e financeiras**.

A aplicação combina a análise e modelagem dos processos **AS-IS e TO-BE** com módulos funcionais de **Estoque, Vendas, Contas a Pagar e Contas a Receber**, permitindo visualizar como processos, dados e sistemas podem trabalhar de forma integrada.

---

## 🎯 Objetivo

Demonstrar como **processos, dados, áreas de negócio e sistemas** podem funcionar de maneira integrada dentro de uma organização.

A solução permite trabalhar com:

- Modelagem do processo atual (**AS-IS**)
- Modelagem do processo futuro (**TO-BE**)
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

Apresenta uma visão consolidada das principais informações da operação, incluindo:

- Produtos cadastrados
- Produtos com estoque baixo
- Quantidade de vendas
- Faturamento
- Valores a pagar
- Valores a receber

### 🏗️ Arquitetura e Processos

O sistema apresenta recursos relacionados à análise de processos empresariais:

- Fluxo AS-IS
- Fluxo TO-BE
- Conceitos de processos de negócio
- Descrição dos procedimentos
- Identificação de gargalos
- Identificação de retrabalho
- Análise de handoffs
- Tratamento de exceções
- Indicadores de desempenho
- Justificativas para as melhorias propostas

### 📦 Estoque

Permite realizar o gerenciamento dos produtos da empresa:

- Cadastro e atualização de produtos
- Código do produto
- Nome do produto
- Categoria
- Quantidade disponível
- Estoque mínimo
- Preço de venda
- Identificação de produtos com estoque baixo
- Atualização do estoque após uma venda

### 🛒 Vendas

Permite registrar as operações comerciais:

- Registro de vendas
- Identificação do cliente
- Seleção do produto
- Quantidade vendida
- Data da venda
- Forma de pagamento
- Cálculo do valor da operação
- Baixa automática da quantidade vendida no estoque

### 💸 Contas a Pagar

Permite controlar as obrigações financeiras da empresa:

- Cadastro de despesas
- Descrição da conta
- Identificação do fornecedor
- Valor
- Data de vencimento
- Acompanhamento da situação do pagamento

### 💰 Contas a Receber

Permite acompanhar os valores que a empresa possui para receber:

- Cadastro de recebíveis
- Identificação do cliente
- Descrição
- Valor
- Data de vencimento
- Acompanhamento da situação do recebimento
- Integração com vendas realizadas a prazo

---

## 🔄 Integração entre os Módulos

Uma das principais características do projeto é a integração entre diferentes operações do sistema.

Por exemplo, ao registrar uma venda, a quantidade vendida é descontada do estoque.

Quando a operação é realizada a prazo, o sistema também pode gerar o respectivo registro em **Contas a Receber**.

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
```

Dessa forma, os módulos representam um **fluxo integrado de informações**, em vez de funcionarem apenas como telas independentes.

---

## 🏗️ AS-IS e TO-BE

A aplicação também apresenta a análise de um processo de **onboarding de fornecedores**, comparando o cenário atual com uma proposta de processo futuro.

### 🔴 AS-IS

O **AS-IS** representa como o processo funciona atualmente.

Entre os principais problemas identificados estão:

- Esperas entre áreas
- Handoffs excessivos
- Reenvio de documentos
- Validações repetidas
- Redigitação de informações
- Dados distribuídos entre diferentes sistemas
- Falta de regras claras para tratamento de exceções

O processo analisado possui um lead time aproximado de **25 dias**, apesar de o trabalho efetivo ser inferior a **4 horas**.

### 🟢 TO-BE

O **TO-BE** representa a proposta de processo futuro após a aplicação das melhorias.

Entre as melhorias propostas estão:

- Portal único para entrada de informações
- Reutilização de dados
- Validações paralelas
- Regras automáticas
- Separação entre casos padrão e exceções
- Fila específica para tratamento de exceções
- Integração com ERP
- Integração com gestão de identidade

O objetivo é reduzir **esperas, retrabalho, redigitação e transferências desnecessárias entre áreas**.

---

## 📊 Indicadores

O sistema utiliza indicadores para acompanhar tanto os processos quanto as operações da empresa.

### Indicadores de processo

- Lead time
- Taxa de retrabalho
- Taxa de automação

### Indicadores operacionais

- Produtos cadastrados
- Produtos com estoque baixo
- Quantidade de vendas
- Faturamento
- Total a pagar
- Total a receber

Os indicadores permitem acompanhar o desempenho e avaliar os resultados das melhorias propostas.

---

## 🧠 Conceitos Aplicados

![Enterprise Architecture](https://img.shields.io/badge/Enterprise%20Architecture-6F42C1?style=for-the-badge)
![BPMN](https://img.shields.io/badge/BPMN-7B61A8?style=for-the-badge)
![AS-IS](https://img.shields.io/badge/AS--IS-555555?style=for-the-badge)
![TO-BE](https://img.shields.io/badge/TO--BE-00A86B?style=for-the-badge)
![Business Process](https://img.shields.io/badge/Business%20Process-5B5FC7?style=for-the-badge)

O projeto aborda conceitos relacionados a:

- Arquitetura Empresarial
- Processos de negócio
- BPMN
- AS-IS
- TO-BE
- Eventos
- Tarefas
- Gateways
- Pools e Lanes
- Handoffs
- Gargalos
- Retrabalho
- Automação
- Tratamento de exceções
- Indicadores de desempenho
- Integração entre processos e sistemas

---

## 🛠️ Tecnologias

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![LocalStorage](https://img.shields.io/badge/LocalStorage-5C5C5C?style=for-the-badge&logo=googlechrome&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)
![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-222222?style=for-the-badge&logo=github&logoColor=white)

A aplicação foi desenvolvida utilizando **HTML, CSS e JavaScript puro**, sem necessidade de frameworks ou dependências externas.

O **LocalStorage** é utilizado para persistir os dados da aplicação diretamente no navegador.

O **GitHub** é utilizado para versionamento e armazenamento do código-fonte, enquanto o **GitHub Pages** é responsável pela publicação da aplicação.

---

## 🧩 Arquitetura da Aplicação

A aplicação utiliza uma arquitetura frontend simples, executada diretamente no navegador.

### Frontend

**HTML5** é responsável pela estrutura e organização dos elementos da aplicação.

### Interface

**CSS3** é responsável pelo layout, responsividade, menu lateral e identidade visual.

### Regras de negócio

**JavaScript** é responsável pelas operações, cálculos, navegação, integrações e comportamento dos módulos.

### Persistência

O **LocalStorage** do navegador é utilizado para armazenar os dados cadastrados durante a utilização da aplicação.

> O projeto não possui backend ou banco de dados externo. Os dados são armazenados localmente no navegador utilizado.

---

## 🔗 Visão da Arquitetura

```text
                    ┌────────────────┐
                    │   DASHBOARD    │
                    └───────┬────────┘
                            │
              ┌─────────────┼─────────────┐
              │             │             │
              ▼             ▼             ▼
          ESTOQUE         VENDAS       FINANCEIRO
              ▲             │             ▲
              │             │             │
              └─────────────┘             │
                 Baixa                    │
               automática                │
                                         │
                          Venda a prazo ──┘
```

Essa estrutura representa a comunicação entre os diferentes módulos da aplicação.

---

## 📂 Estrutura do Projeto

```text
sistema-gestao-empresarial/
│
├── index.html
└── README.md
```

O projeto foi desenvolvido em um único arquivo `index.html`, que concentra:

- Estrutura HTML
- Estilização CSS
- Lógica JavaScript
- Navegação
- Regras de negócio
- Persistência local
- Modelagem dos processos
- Módulos operacionais e financeiros

---

## 💾 Persistência dos Dados

Os registros realizados na aplicação são armazenados utilizando o **LocalStorage** do navegador.

Isso permite que os dados permaneçam disponíveis mesmo após atualizar ou fechar a página, desde que o usuário utilize o mesmo navegador e os dados locais não sejam apagados.

Como o projeto não possui servidor ou banco de dados externo, os registros não são compartilhados entre diferentes dispositivos ou navegadores.

---

## ▶️ Como Executar

### 🌐 Online

A aplicação está publicada através do GitHub Pages:

[![Acessar Sistema](https://img.shields.io/badge/Acessar-Sistema%20Online-00C7B7?style=for-the-badge)](https://juliamergulhao.github.io/sistema-gestao-empresarial/)

### 💻 Localmente

1. Clone ou faça o download deste repositório.
2. Localize o arquivo `index.html`.
3. Abra o arquivo em um navegador.
4. O sistema estará pronto para utilização.

Não é necessária a instalação de dependências.

---

## 🎓 Contexto Acadêmico

Projeto desenvolvido no contexto da disciplina de **Arquiteturas Empresariais**, com foco na análise ponta a ponta de processos de negócio.

O trabalho envolve a identificação do processo atual (**AS-IS**), seus problemas e oportunidades de melhoria, seguida pela elaboração de um processo futuro (**TO-BE**) com simplificação, automação e integração.

Além da modelagem dos processos, foram implementados módulos operacionais para demonstrar como **processos, dados, sistemas e áreas de negócio podem funcionar de maneira integrada**.

---

Projeto desenvolvido para estudo e aplicação prática de conceitos de **Arquitetura Empresarial, Processos de Negócio e Sistemas de Gestão**.
