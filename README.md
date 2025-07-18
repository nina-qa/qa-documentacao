## 📂 Visão Geral da Documentação de Qualidade de Software

💡 Introdução

A documentação na área de Qualidade de Software (QA) é essencial para garantir a rastreabilidade, a compreensão do escopo, a reprodutibilidade de testes e a comunicação eficiente entre times. Uma boa documentação ajuda a padronizar processos, mitigar riscos e acelerar a detecção de falhas.

📄 Importância da Documentação em QA

Rastreabilidade: ligação entre requisitos, casos de teste e defeitos.

Histórico: registro das versões testadas e comportamentos esperados.

Colaboração: facilita a entrada de novos membros e a comunicação com stakeholders.

Eficiência: evita retrabalho ao ter casos de teste reutilizáveis.

Auditoria: garante conformidade com padrões e regulamentações.

01-Testes-Manuais

Contém o README.md com definições, objetivos, aplicações e exemplos dos principais tipos de testes manuais:

Teste Funcional

Teste de Regressão

Teste Exploratorio

Teste de Interface (UI)

Teste de Aceitação (UAT)

Smoke Test

Sanity Test

02-Testes-Automatizados

Documentação para testes automatizados utilizando o framework Cypress, com base em JavaScript/TypeScript.

Inclui:

Stack (Cypress, JS/TS, CI, Allure)

Tipos de testes abordados: Regressão, Funcional, Smoke, Integração de Frontend e E2E

Estrutura do projeto Cypress:

/cypress

├── e2e         # Casos de teste organizados por feature

├── fixtures    # Dados simulados (mock)

├── support     # Comandos customizados e configurações

└── reports     # Resultados e evidências dos testes


Exemplo real de script de teste Cypress (login)

Comandos para execução via terminal

Geração de relatórios com Allure

Esse material é útil para profissionais que desejam iniciar ou manter uma base sólida em automação de testes frontend.

🔌 03-Testes-API

Documentação para testes de APIs REST utilizando Postman (manual) e Newman (automação CLI).

Inclui:

Tipos de testes: Contrato, Status Code, Performance, Autenticação, Erros

Estrutura de projeto:

/postman

├── collections     # Coleções de requisições

├── environments    # Variáveis por ambiente

└── tests           # Scripts de validação

Exemplos de scripts com pm.test para Postman

Comando para rodar coleções com Newman

Geração de relatórios HTML via linha de comando

Ideal para validar a camada de comunicação entre serviços e detectar falhas de backend, segurança e estrutura.
