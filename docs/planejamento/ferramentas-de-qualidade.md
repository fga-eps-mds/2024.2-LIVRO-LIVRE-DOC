# Plano de Qualidade

## Versão

|    Data    | Versão |      Descrição       |                                                        Autor                                                     |
|:----------:|:------:|:--------------------:|:----------------------------------------------------------------------------------------------------------------:|
| 09/12/2024 |  1.0   | Criação do documento | Mateus Maia  |

## Introdução

A qualidade é um aspecto fundamental em qualquer projeto de software. Para garantir que nosso projeto atenda aos mais altos padrões de qualidade, criamos um plano que adota tecnologias e práticas eficazes para aprimorar a qualidade do código, a robustez da aplicação e a confiabilidade do software. Este plano de qualidade descreve como planeja-se a utilização de métricas e tecnologias de suporte para assegurar a qualidade do projeto.

## Ferramentas

| Ferramenta  | Descrição                       |
| ----------- | ------------------------------- |
| Sonar Cloud | Ferramenta de análise de código |
| Jest        | Framework de testes JavaScript   |

## SonarCloud

O **SonarCloud** é uma ferramenta de análise de código estático que oferece insights valiosos sobre a qualidade do código, detectando problemas, vulnerabilidades e áreas que necessitam de melhorias. A integração dessa ferramenta ao processo de desenvolvimento é essencial para manter a qualidade do projeto.

### Detalhes do uso do SonarCloud:

- **Análise Contínua de Código**: A cada commit, pull request ou build, a ferramenta executa uma análise automática do código, ajudando a detectar problemas em tempo real.
  
- **Identificação de Vulnerabilidades e Erros**: O SonarCloud é capaz de identificar vulnerabilidades de segurança, bugs e outras falhas no código.

- **Métricas de Qualidade**: Acompanhamos indicadores importantes como cobertura de código, complexidade e duplicação de código, a fim de manter o código eficiente e limpo.

- **Integração no Fluxo de Trabalho**: A integração do SonarCloud com o fluxo de trabalho de desenvolvimento possibilita a revisão e correção de problemas durante o ciclo de desenvolvimento, promovendo melhorias contínuas na qualidade do código.

## Jest

O **Jest** é um framework de testes para JavaScript, amplamente usado para garantir que os componentes de aplicações, tanto do front-end quanto do back-end, funcionem corretamente. Ele é uma parte essencial para garantir a integridade e o funcionamento correto do software.

### Detalhes do uso do Jest:

- **Testes Unitários e de Integração**: O Jest será utilizado para criar testes unitários e de integração, assegurando que tanto os componentes front-end em React quanto os módulos de back-end em Nest estejam funcionando corretamente.

- **Testes Automatizados**: Uma suíte de testes automatizados será configurada e executada em um ambiente de integração contínua sempre que houver alterações no código.

- **Cobertura de Testes**: Monitoraremos a cobertura de testes para garantir que uma grande parte do código seja testada, identificando eventuais áreas que ainda necessitem de testes.

- **Testes de Desempenho**: Implementaremos testes focados no desempenho para garantir que o software seja eficiente e responsivo, principalmente em cenários com alta carga.

## Testes Unitários

Os **testes unitários** são realizados para avaliar o comportamento das menores unidades do código, como funções ou métodos. Eles verificam se as entidades individuais do sistema, como classes ou funções, estão funcionando de acordo com o esperado, independentemente das outras partes do sistema.

## Testes de Integração

Diferente dos testes unitários, os **testes de integração** verificam como diferentes componentes do sistema interagem entre si. Eles são essenciais para identificar falhas nas interfaces de comunicação entre módulos, garantindo que o sistema funcione de forma integrada e que os componentes colaboram corretamente para a execução das funcionalidades.

## Testes E2E (End to End)

Os **testes E2E (End to End)** avaliam o sistema como um todo, verificando se o fluxo da aplicação funciona de maneira integrada, desde a interface do usuário até o banco de dados. Com esses testes, garantimos que a experiência do usuário seja fluida e sem problemas, identificando falhas em cenários mais próximos da realidade do usuário final.

## Referências

> [**SONAR CLOUD**](https://www.sonarsource.com/products/sonarcloud).

> [**JEST**](https://jestjs.io/pt-BR/)