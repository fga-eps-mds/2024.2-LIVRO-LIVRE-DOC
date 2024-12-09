# Javascript
## Histórico de Versões

| **Título**                   | **Alterações Feitas**                  | **Autor**      | **Data de Hoje**         |
|------------------------------|----------------------------------------|----------------|--------------------------|
| Dojo de javascript v1       | Subindo documento versão 1             | Matheus Monteiro    | 08 de dezembro de 2024   |


## Introdução

Bem-vindo ao treinamento básico de JavaScript com Node.js 20, focado no desenvolvimento de APIs backend! Neste curso, exploraremos como construir uma API simples e eficiente, sem o uso de frameworks de terceiros, para que você compreenda os conceitos fundamentais do Node.js e a arquitetura de APIs.
## Objetivo do Treinamento
O principal objetivo é capacitar você a criar uma API que gerencie a jornada de um usuário, coletando informações básicas, como nome e email. Durante o treinamento, abordaremos tópicos essenciais para a construção de APIs robustas e escaláveis.

### Módulo 1: Configuração do Ambiente
- **Instalação do Node.js**: Explicação passo a passo para instalar o Node.js, garantindo que você tenha o ambiente adequado.

- **Configuração do Projeto**: Criação do projeto do zero, incluindo a estrutura básica de pastas e arquivos.

- **Testando o Ambiente**: Execução de um teste simples para confirmar que o Node.js está configurado corretamente.
### Módulo 2: Entendendo o Conceito de Middlewares
- **Definição e Função de Middlewares**: O que são middlewares e como eles interceptam e manipulam as requisições.

- **Implementação de Middlewares**: Como criar e configurar middlewares básicos para tratamento de erros e autenticação, se necessário.
### Módulo 3: HTTP e Métodos
- **Explicação dos Verbos HTTP**:
- **GET**: Recupera informações.
- **POST**: Cria uma nova entrada no servidor.
- **PUT**: Atualiza uma entrada existente.
- **PATCH**: Atualiza apenas um campo específico de uma entrada.
- **DELETE**: Exclui uma entrada do servidor.
- **Comando CURL**: Demonstração do uso do `curl` para testar a API:
- Exemplo: `curl -X POST http://localhost:3333/users` para criação de um usuário.
### Módulo 4: Estruturação da API
- **Organização do Código**: Dicas e práticas para separar responsabilidades, facilitando a manutenção do código.
- **Estrutura de Pastas e Arquivos**: Padrões para organizar controladores, modelos e serviços de forma que o projeto seja claro e sustentável.
- **Conceitos de Arquitetura REST**: Introdução aos princípios REST que vamos implementar na API.
### Módulo 5: Manipulação de Requisições e Respostas
- **Introdução às Rotas**: Como criar rotas básicas para que o servidor responda às solicitações do usuário.
- **Conceito de Requisição e Resposta**: Explicação sobre os objetos `request` e `response`, que representam as interações entre cliente e servidor.
- **Criando Endpoints Básicos**:
	- **GET**: Recuperação de informações.
	- **POST**: Inserção de dados.
	- **PUT** e **PATCH**: Atualização de dados (diferenças entre esses métodos).
	- **DELETE**: Remoção de dados.
	
### Módulo 6: Persistência de Dados com Node.js
- **Uso de Arquivos com o Módulo FS**:
	Como manipular arquivos em Node.js utilizando `import fs from 'node:fs/promises'`. Armazenamento de dados em arquivos locais para simular um banco de dados.
- **CRUD Completo**:
	- **Create (POST)**: Como salvar novos dados.
	- **Read (GET)**: Como recuperar dados existentes.
	- **Update (PUT/PATCH)**: Atualização de informações.
	- **Delete (DELETE)**: Remoção de registros.
### Projeto Final: Construindo o CRUD
  
- **Construção da Tabela `users`**:
- Estrutura de uma tabela simples para armazenar dados de usuários.
- **Implementação do CRUD Completo**:
- Desenvolvendo o CRUD completo com os métodos HTTP aprendidos, usando apenas JavaScript e Node.js.
- Testando o CRUD usando Insomnia ou Postman e analisando as respostas da API.
## Referências e Materiais de Apoio

1. **[Rocketseat - Projeto básico de API com Node.js](https://app.rocketseat.com.br/classroom/projeto-01-1)**: Projeto de criação de uma aplicação Node.js sem frameworks.

2. **[Documentação do JavaScript - Mozilla MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript)**: Documentação oficial do JavaScript, cobrindo desde sintaxe até funções avançadas.

3. **[Artigo Alura - Como funciona o Node.js](https://www.alura.com.br/artigos/node-js)**: Introdução ao funcionamento e fluxo de trabalho no Node.js.

4. **[Node.js - Motor V8 JavaScript](https://nodejs.org/en/learn/getting-started/the-v8-javascript-engine)**: Explicação do motor JavaScript V8, que executa o código do Node.js.

5. **[Node.js - Buffer API](https://nodejs.org/api/buffer.html#buffer)**: Funcionamento e uso do buffer em Node.js.
