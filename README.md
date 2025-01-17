Testes E2E com Cypress

Este projeto utiliza o Cypress para realizar testes de ponta a ponta (E2E), validando a funcionalidade de uma aplicação. A automação cobre os seguintes cenários:

🚀 Funcionalidades Testadas
Validação da Página Inicial

Verifica se a página inicial é carregada corretamente e se todos os elementos essenciais estão visíveis e funcionais.
Registro de Novo Usuário

Preenche automaticamente os campos do formulário com dados aleatórios.
Valida o endereço com base no CEP informado.
Seleciona um serviço aleatório disponível.
Realiza o upload de um arquivo como parte do processo de cadastro.
Verifica se a mensagem de sucesso é exibida após o envio do formulário.

📦 Requisitos

Node.js (versão 14 ou superior)
NPM ou Yarn
Cypress instalado no projeto

🔧 Como Executar os Testes
Clone este repositório:

bash
git clone https://gitlab.com/09Igor/cypress-wakdog-automation.git
cd cypress-wakdog-automation

Instale as dependências do projeto:

bash
npm install

Execute os testes em modo interativo:

bash
npx cypress open
Ou, para rodar os testes diretamente no terminal:

bash
npx cypress run

🛠 Tecnologias Utilizadas

Cypress: Framework para testes E2E.
Faker.js: Geração de dados aleatórios para simulação de entradas de usuário.
Node.js: Ambiente de execução para JavaScript.

📂 Estrutura do Projeto
plaintext

cypress-wakdog-automation/
├── cypress/
│   ├── fixtures/          # Arquivos estáticos (ex.: dados de teste)
│   ├── integration/       # Testes E2E
│   │   ├── home.spec.js   # Teste de validação da página inicial
│   │   └── register.spec.js # Teste de registro de novo usuário
│   ├── plugins/           # Configurações de plugins do Cypress
│   └── support/           # Comandos customizados e configurações globais
├── package.json           # Dependências do projeto
└── README.md              # Documentação do projeto

📋 Próximos Passos
 
- Adicionar testes para validação de cenários negativos (ex.: campos obrigatórios ausentes).
- Automatizar execução de testes em CI/CD usando GitLab Pipelines.
- Melhorar a cobertura dos testes com cenários adicionais.
