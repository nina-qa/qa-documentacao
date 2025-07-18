# 🤖 Testes Automatizados

Automatizar testes garante velocidade, repetibilidade e confiabilidade. Utilizamos **Cypress** como framework principal de automação.

## 🧰 Stack

- Cypress
- JavaScript / TypeScript
- GitHub Actions (CI)
- Allure Reports

## 📌 Tipos de Testes Automatizados

- **Teste de Regressão**
- **Teste Funcional**
- **Smoke Test**
- **Testes de Integração Frontend**
- **Testes E2E (End-to-End)**

## 📂 Estrutura dos Arquivos

/cypress

├── e2e

├── fixtures

├── support

└── reports


## 🔄 Exemplo de Teste

```js
describe('Login', () => {
  it('deve logar com sucesso', () => {
    cy.visit('/login');
    cy.get('#email').type('teste@email.com');
    cy.get('#senha').type('123456');
    cy.get('button[type="submit"]').click();
    cy.url().should('include', '/dashboard');
  });
});

