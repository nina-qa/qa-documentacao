
 🔌 Testes-API/README.md

```markdown
# 🔌 Testes de API

Testes de API são essenciais para validar a comunicação entre serviços. Usamos o **Postman** para testes exploratórios e o **Newman** para automação via CLI.

## 📌 Tipos de Teste de API

- **Teste de Contrato**
- **Teste de Status Code**
- **Teste de Performance**
- **Teste de Autenticação**
- **Teste de Erros**

## 📂 Estrutura de Coleções

/postman

├── collections

├── environments

└── tests


## 🔍 Exemplo de Teste (Postman)

```js
pm.test("Status code is 200", function () {
    pm.response.to.have.status(200);
});

pm.test("Body contains username", function () {
    const jsonData = pm.response.json();
    pm.expect(jsonData.username).to.eql("admin");
});
