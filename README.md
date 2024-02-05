#Automação de Testes com Cypress

## Índice

- [Visão Geral](#visão-geral)
- [Testes Implementados](#testes-implementados)
  - [Cadastro de Usuários](#cadastro-de-usuários)
  - [Login de Usuários](#login-de-usuários)
  - [Interação com APIs](#interação-com-apis)
  - [Testes Flaky](#testes-flaky)
  - [Testes Gerais](#testes-gerais)
- [Técnicas de Teste](#técnicas-de-teste)
  - [Testes de Integração](#testes-de-integração)
  - [Testes de UI](#testes-de-ui)
  - [Stubbing e Interceptação de Rede](#stubbing-e-interceptação-de-rede)
- [Execução dos Testes](#execução-dos-testes)
- [Relatórios de Testes](#relatórios-de-testes)
- [Contribuição](#contribuição)
- [Licença](#licença)
- [Contato](#contato)

## Visão Geral

Este repositório contém uma coleção de testes automatizados para uma aplicação web, utilizando o framework Cypress. Os testes foram projetados para validar a funcionalidade e a segurança da aplicação, cobrindo desde o cadastro e login de usuários até a interação com APIs e a consistência de dados.

## Testes Implementados

### Cadastro de Usuários

- **Cadastro com Dados Válidos**: Verifica se o sistema permite o cadastro de novos usuários com informações válidas.
- **Cadastro em Massa**: Utiliza um conjunto de dados de usuários para testar o cadastro em massa.
- **Validação de Campos de Cadastro**: Confirma se o sistema exibe mensagens de erro apropriadas quando os campos obrigatórios estão vazios.

### Login de Usuários

- **Login com Dados Corretos**: Assegura que o login funcione corretamente com credenciais válidas.
- **Login com Dados Incorretos**: Garante que o sistema rejeite logins com credenciais inválidas e mostre mensagens de erro.
- **Stubbing de Login**: Emprega interceptação de rede para simular diferentes respostas do servidor durante o processo de login.

### Interação com APIs

- **Buscar Fotos e Dados**: Faz requisições GET para verificar se as fotos e dados dos usuários são retornados corretamente pela API.
- **Dados Seguros**: Realiza o login via API e verifica a segurança e a correção dos dados retornados.

### Testes Flaky

- **Buscar Fotos com Tempo Variável**: Testa a consistência das respostas da API sob condições de rede variáveis.

### Testes Gerais

- **Navegação e Registro**: Verifica a navegação para a página de cadastro e o preenchimento correto dos campos.
- **Teste Básico de Acesso**: Confirma se a aplicação está acessível visitando a URL base.

## Técnicas de Teste

### Testes de Integração

- **Cypress Fixtures**: Utiliza dados pré-definidos para simular o comportamento do usuário e a interação com a aplicação.

### Testes de UI

- **Element Traversal**: Emprega seletores para interagir com elementos da interface do usuário e validar estados e comportamentos.

### Stubbing e Interceptação de Rede

- **Cypress Intercept**: Intercepta chamadas de rede para testar o comportamento da aplicação com diferentes respostas do servidor.

## Execução dos Testes

Para executar os testes, use o comando `npx cypress open` para o modo interativo ou `npx cypress run` para o modo headless.

## Relatórios de Testes

Os relatórios são gerados pelo Mochawesome e podem ser encontrados no diretório de relatórios configurado no Cypress.

## Contribuição

Contribuições para melhorar os testes ou a cobertura de testes são bem-vindas. Por favor, faça um fork do repositório, faça suas alterações e envie um pull request.

## Licença

Este projeto é licenciado sob a Licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

## Contato

Para dúvidas ou sugestões, entre em contato através dos meios fornecidos
