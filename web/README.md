# 🧪 Testes Automatizados -- Webdojo (Cypress)

Este repositório contém a aplicação **Webdojo** e sua suíte de **testes
automatizados utilizando Cypress**.\
A aplicação e os testes convivem no mesmo projeto para facilitar o
desenvolvimento, manutenção e execução local.

## 📁 Estrutura do Projeto

A imagem abaixo representa a estrutura principal da pasta `cypress`:

    cypress/
     ├── e2e/
     │    ├── fixtures/
     │    │     ├── cep.json
     │    │     ├── consultancy.json
     │    │     └── document.pdf
     │    │
     │    └── ...
     │
     ├── support/
          ├── actions/
          │     └── consultancy.actions.js
          ├── commands.js
          ├── e2e.js
          └── utils.js

### 📂 Descrição das Pastas

  -----------------------------------------------------------------------
  Pasta/Arquivo                                      Descrição
  -------------------------------------------------- --------------------
  **cypress/e2e**                                    Contém os arquivos
                                                     de testes end-to-end
                                                     (E2E).

  **cypress/e2e/fixtures**                           Massa de dados usada
                                                     nos testes (JSON,
                                                     PDF, etc.).

  **cypress/support**                                Conjunto de
                                                     utilitários e
                                                     configurações
                                                     globais do Cypress.

  **actions**                                        Arquivos que
                                                     encapsulam
                                                     interações com a
                                                     aplicação (Page
                                                     Actions).

  **commands.js**                                    Comandos
                                                     customizados do
                                                     Cypress.

  **e2e.js**                                         Setup global
                                                     executado antes dos
                                                     testes.

  **utils.js**                                       Funções utilitárias
                                                     reutilizáveis.
  -----------------------------------------------------------------------

## 🚀 Executando a Aplicação Webdojo

Antes de rodar os testes, execute a aplicação localmente:

``` bash
npm run dev
```

O comando acima inicia a versão compilada do Webdojo utilizando o pacote
`serve` na porta **3000**.

## 🧪 Executando os Testes

Os scripts abaixo estão definidos no `package.json`:

### ▶️ Rodar todos os testes em modo headless

``` bash
npm test
```

### 🖥️ Abrir o Cypress em modo interativo (UI)

``` bash
npm run test:ui
```

### 🔐 Rodar somente os testes de login

``` bash
npm run test:login
```

### 📱 Rodar testes de login em viewport mobile

``` bash
npm run test:login:mobile
```

## 🧱 Padrão de Organização

### ✳️ Fixtures

Localizados em `cypress/fixtures`.

### ⚙️ Actions (Page Actions)

Funções encapsuladas em `cypress/support/actions/`.

### 🔧 Commands Customizados

Localizados em `cypress/support/commands.js`.

### 🧩 Utils

Localizados em `cypress/support/utils.js`.

## 📌 Boas Práticas Utilizadas

-   Organização dos testes por funcionalidade\
-   Separação de Page Actions\
-   Uso de fixtures\
-   Commands customizados\
-   Configuração padronizada de viewport\
-   Testes separados entre desktop e mobile

## 📄 Requisitos

-   Node.js instalado\
-   Cypress instalado\
-   Aplicação Webdojo rodando (`npm run dev`)

## 📬 Contato / Contribuição

Pull requests, issues e sugestões são bem-vindos.
