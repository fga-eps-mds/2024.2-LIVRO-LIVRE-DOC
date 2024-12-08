---
sidebar_position: 1
---

# Início

Wiki destinada ao projeto Livre Livro contendo toda a documentação referente à disciplina de Engenharia de Produto de Software (EPS) e Métodos de Desenvolvimento de Software (MDS) durante o semestre de 2024.2, ministrada pelo professor Hilmer Rodrigues Neri da Universidade de Brasília - Gama.

## Equipe

PREENCHER COM NOMES E IMAGENS DA EQUIPE


# Documento de Arquitetura

## Histórico de Revisão

| Data       | Versão | Modificação                                    | Autor              |
|------------|--------|------------------------------------------------|--------------------|
| 08/12/2024 | 0.1    | Criação do documento                           | Jonas Carlos        |
| 08/12/2024 | 0.2    | Criação dos topicos 1 e 2                      | Jonas Carlos        |

---

## 1. Introdução

### 1.1 Finalidade
Este documento de arquitetura tem como objetivo formalizar e registrar as decisões arquiteturais essenciais para a produção e implementação do projeto "Livro Livre". O software tem a finalidade de gerenciar e catalogar o acervo de livros nas estantes do projeto, controlando quais livros estão disponíveis e quais estão em uso, proporcionando um gerenciamento simples e eficiente.

### 1.2 Escopo
Este documento cobre o processo de desenvolvimento da aplicação, na qual será possível visualizar os livros cadastrados, cadastrar novos livros, verificar o status de disponibilidade (em uso ou disponível) e os detalhes relacionados a cada título. A aplicação será acessada por usuários que desejam consultar e pegar livros emprestados, sem custos ou prazos de devolução definidos.

As visões contempladas para esse modelo são:
- Visão de Casos de Uso;
- Visão Lógica.

---

## 2. Representação da Arquitetura

Modelo de representação dos serviços implementados e as interações estabelecidas entre esses serviços, bem como a natureza dessas interações.
### 2.1 Tecnologias

#### 2.1.1 Front End
**React**  
O React foi escolhido para a construção da interface do usuário devido à sua flexibilidade, eficiência e suporte a componentes reutilizáveis. Sua popularidade também facilita a manutenção e a implementação de novas funcionalidades no sistema.

**HTML, CSS e JavaScript**  
HTML e CSS são utilizados para estruturar e estilizar a interface, enquanto JavaScript complementa a interação do usuário no front-end, garantindo uma experiência dinâmica e responsiva.

#### 2.1.2 Back End
**Node.js**  
O Node.js foi selecionado para o back-end devido à sua performance e escalabilidade. Ele permite que a aplicação manipule requisições de forma eficiente, utilizando a abordagem orientada a eventos e assíncrona do Node.js.

**Python**  
Python pode ser utilizado em componentes específicos do sistema, como scripts de automação ou para tarefas de processamento de dados, dados que não exigem alta performance em tempo real, mas que são importantes para o gerenciamento do sistema.

#### 2.1.3 Banco de Dados
**PostgreSQL**  
O PostgreSQL foi escolhido como banco de dados devido à sua robustez e confiabilidade no armazenamento de dados estruturados, como informações sobre livros, usuários e status de locação. Além disso, oferece suporte a consultas complexas e garante integridade transacional, o que é essencial para garantir a precisão no gerenciamento de dados de locação.

---




