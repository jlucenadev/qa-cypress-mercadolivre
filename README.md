# 🛒 Automação Mercado Livre com Cypress + JavaScript

Este projeto apresenta uma automação completa do Mercado Livre utilizando **Cypress + JavaScript**, cobrindo fluxos reais de e-commerce como busca, aplicação de filtros, validação de preços e detalhes de produtos.

Criado para servir como **projeto de portfólio profissional para QA Automation**.

---

## 🚀 Tecnologias Utilizadas

- **Cypress 13**
- **JavaScript (ES6)**
- **Node.js**
- **Page Object Model (POM)**
- **Faker.js** (massa de dados fake, opcional)
- **GitHub Actions (opcional para CI/CD)**

---

## 🎯 Objetivo da Automação

Demonstrar domínio de automação web em um site real, dinâmico e amplamente utilizado, validando:

- Busca de produtos
- Aplicação de filtros (preço e condição)
- Abertura de anúncio
- Comparação de preço entre lista e página interna
- Validação de elementos dinâmicos
- Fluxos com seletores estáveis e boas práticas

---

## 🧪 Cenários Automatizados

### ✔ **1. Busca de produto**
- Digitar termo de busca (ex.: *iPhone 15*)
- Validar que os resultados aparecem
- Validar título da página
- Garantir que os cards exibem nome e preço

### ✔ **2. Aplicar filtros**
- Filtrar por condição (Novo)
- Filtrar por faixa de preço
- Validar se todos os resultados atendem ao filtro
- Garantir que não existem preços fora da faixa

### ✔ **3. Abrir detalhes de um produto**
- Clicar no primeiro item
- Validar nome do produto
- Validar preço interno
- Validar selo “Novo”, quando aplicável

### ✔ **4. Comparação de preço**
- Capturar preço no card da listagem
- Capturar preço na página do produto
- Validar se os valores coincidem

---

## 📁 Estrutura do Projeto

```
qa-cypress-mercadolivre/
 ├─ cypress/
 │   ├─ e2e/
 │   │    ├─ search.cy.js
 │   │    ├─ filters.cy.js
 │   │    ├─ productDetails.cy.js
 │   ├─ pages/
 │   │    ├─ HomePage.js
 │   │    ├─ SearchResultsPage.js
 │   │    ├─ ProductPage.js
 │   ├─ fixtures/
 │   │    ├─ searchTerms.json
 │   └─ support/
 │        ├─ commands.js
 │        └─ e2e.js
 ├─ cypress.config.js
 ├─ package.json
 └─ README.md
```

### **Padrões utilizados**
- Page Object Model para separar páginas dos testes
- Testes limpos e reutilizáveis
- Seletores estáveis (evitando IDs dinâmicos)
- Validações robustas com `.should()`
- Estrutura para CI/CD compatível com GitHub Actions

---

## ▶️ Como Rodar o Projeto

### **1. Instalar dependências**
```
npm install
```

### **2. Abrir o Cypress**
```
npx cypress open
```

### **3. Executar em modo headless**
```
npx cypress run
```

---

## 📸 Evidências

- Screenshots automáticos em caso de falha  
- Vídeos gerados automaticamente quando executado em modo headless  

Os arquivos ficam em:

```
cypress/screenshots/
cypress/videos/
```

---

## 🧱 Padrões de Código (Boas Práticas)

- Page Object Model (POM)
- Testes independentes e idempotentes
- Uso de `beforeEach` para iniciar cenários limpos
- Seletores confiáveis (`data-testid`, textos e estruturas estáveis)
- Separação clara entre **Page**, **Test** e **Fixtures**

---

## 🔥 Melhorias Futuras

- Adicionar CI/CD com GitHub Actions  
- Integrar relatório Allure  
- Cobrir fluxo de login real (quando disponível)  
- Adicionar testes de interceptação de rede (API + UI)  

---

## 👤 Autor

**Josué Lucena**  
QA Automation | Cypress | JavaScript  
