# Dojo NestJS: Construindo Backends Escaláveis e Eficientes em TypeScript

## Versão

| **Título**        | **Alterações Feitas**                         | **Autor**  | **Data de Hoje**       |
|-------------------|-----------------------------------------------| -----------| ---------------        |
| Dojo Rest.js   | Subindo documento versão 1                    | Mateus Maia | 09 de dezembro de 2024 |


## Introdução ao NestJS

* **O que é NestJS?**
    Um framework Node.js progressivo que utiliza TypeScript, oferecendo uma estrutura robusta para a construção de aplicações back-end escaláveis e eficientes.
* **Por que usar NestJS?**
    * **TypeScript:** Tipagem estática, melhorando a qualidade do código.
    * **Modularidade:** Organização em módulos, promovendo reutilização.
    * **Dependecy Injection:** Injeção de dependências automática.
    * **Comunidade:** Grande comunidade e suporte.
    * **Performance:** Otimizado para alto desempenho.

## Instalando e Configurando o Ambiente

* **Instalação:**
    ```bash
    npm install -g @nestjs/cli
    nest new my-nest-app
    cd my-nest-app
    npm run start
    ```
* **Editor de código:** Visual Studio Code, Sublime Text, Atom.
* **Extensões:** TypeScript, ESLint, Prettier.

## Conceitos Fundamentais

* **Módulos:** Contêm controladores, serviços, provedores.
* **Controladores:** Exportam rotas HTTP.
* **Serviços:** Contêm a lógica de negócio.
* **Provedores:** Fornecem serviços para outras partes da aplicação.
* **Decoradores:** Adicionam metadados às classes.
* **Pipes:** Validam e transformam dados de entrada.
* **Guards:** Protegem rotas.
* **Interceptors:** Interceptam requisições e respostas.

## Criando sua Primeira API

* **Criando um controlador:**
    ```typescript
    import { Controller, Get } from '@nestjs/common';

    @Controller()
    export class AppController {
      @Get()
      getHello(): string {
        return 'Hello World!';
      }
    }
    ```
* **Testando a API:**
    ```bash
    curl http://localhost:3000
    ```

## Trabalhando com Banco de Dados

* **TypeORM:** ORM popular para NestJS.
* **Mongoose:** Outro ORM popular, especialmente para MongoDB.
* **Criando entidades:**
    ```typescript
    import { Entity, PrimaryGeneratedColumn, Column } from 'typeorm';

    @Entity()
    export class User {
      @PrimaryGeneratedColumn()
      id: number;

      @Column()
      firstName: string;
    }
    ```

## Testando sua Aplicação

* **Jest:** Framework de testes JavaScript.
* **Supertest:** Biblioteca para testar APIs HTTP.

## Tópicos Avançados

* **WebSockets:** Comunicação em tempo real.
* **GraphQL:** Linguagem de consulta para APIs.
* **Microserviços:** Construindo aplicações distribuídas.
* **Cloud Computing:** Deploy em plataformas como AWS, GCP e Azure.

## Projetos Práticos

* **API REST para um blog:** Crie posts, comentários, usuários.
* **Aplicativo de chat em tempo real:** Utilize WebSockets.
* **E-commerce:** Carrinho de compras, pagamentos, produtos.

## Recursos Adicionais

* **Documentação Oficial:** https://nestjs.com/
* **TypeORM:** https://typeorm.io/
* **Mongoose:** https://mongoosejs.com/


