# Metodologias

## Versão 

| **Título**        | **Alterações Feitas**                         | **Autor**  | **Data de Hoje**       |
|-------------------|-----------------------------------------------| -----------| ---------------        |
| Metodologias v1     | Abertura de documento                         | Bruno Cruz | 07 de dezembro de 2024 |
| Metodologias v1.1     | Correção de documento                        | Bruno Cruz | 07 de janeiro de 2025 |

## Introdução

As **metodologias** utilizadas durante todo o processo do desenvolvimento do projeto Livro Livro serão descritas neste documento. Essas metodologias foram usadas para auxiliar esse desenvolvimento, essas podem ser ditas como metodologias ágeis, com objetivo de ciclos de entrega rápidos, contínuos e incrementais, tais como Lean Inception, XP e Scrum.

## Lean Inception

O Lean Inception é uma metodologia colaborativa usada para alinhar equipes e stakeholders na definição de um Mínimo Produto Viável (MVP) de um produto ou serviço. Ela combina práticas do Lean Startup e do Design Thinking para garantir que o produto inicial entregue ao mercado seja viável, útil e alinhado às necessidades dos usuários e do negócio.

## XP​
O método XP (Extreme Programming) descreve um método voltado principalmente para o desenvolvimento de Software, onde neste há um conjunto de práticas de programação. E o objetivo principal do XP é levar ao extremo esse conjunto de práticas, que são ditas como boas na engenharia de software. Algumas dessas usadas no desenvolvimento do Livro Livre são:

### <i>Programação em Par​</i>

A programação em par é feita de modo em que dois programadores desenvolvem uma mesma parte do código em conjunto, no mesmo ambiente. Isso garante com que ambos possam ter o aprendizado sobre cada elemento realizado no projeto, minimizando a dependência de um único colaborador. Também favorece o nivelamento técnico e o compartilhamento de conhecimento em ambos programadores.

A equipe a utilizou separando a equipe em pares para a realização das tarefas, onde a cada sprint esse pareamento foi alterado.  

### <i>Testes de aceitação​​</i>

O Teste de aceitação é um teste funcional, no qual o usuário decidirá se a implementação do produto disponibilizada pela equipe está aceitável, conforme os critérios de aceitação. Esses testes de aceitação podem ocorrer de modo assíncrono, ou no momento da reunião com os PO's.

### <i>Cliente Presente​​</i>

O cliente é participativo no processo do desenvolvimento do Produto, sempre está em contato com os desenvolvedores, observando o processo e recebendo os resultados de cada processo constantemente. 

### <i>Código Coletivo​​</i>

O código-fonte é disponibilizado a todos e todos têm acesso e direito para realizar mudanças. Assim, toda a equipe de desenvolvedores pode conhecer todas as partes do produto. Além da realização da padronização de código do produto.

### <i>Refatoração</i>

A refatoração é o processo de alteração do código-fonte, de uma forma onde esse processo não altere a funcionalidade externa do produto, mas que melhore a estrutura interna do código. A refatoração é usada para termos um código mais limpo e organizado, minimizando o risco de bugs e melhorando o entendimento.

### <i>Releases Curtos​​</i>

Sempre são liberadas pequenas versões do produto para o cliente, assim ele poderá testar partes do produto à medida que este é construído e ajudar no processo de validação. 


### <i>Testes Unitários</i>

Testes unitários são testes realizados em cada elemento do produto, a fim de verificar se cada um deste funciona como o esperado. Esses testes são usados para que seja possível reduzir o risco de propagação de erros, ou até mesmo isolar um erro específico e assim poder realizar a manutenção do código da melhor maneira.

## Scrum

O Scrum é um método ágil voltado para o gerenciamento de projetos, com ênfase na organização e colaboração da equipe. Ele utiliza práticas Scrum, que estruturam o planejamento e a execução das tarefas dos membros da equipe. Esse método promove um fluxo de trabalho contínuo por meio de ciclos iterativos e incrementais chamados sprints. 

Cada sprint tem uma duração predefinida, geralmente de uma semana nesse projeto, durante a qual a equipe trabalha em tarefas prioritárias para entregar um incremento do produto. Ao final de cada sprint, ocorre uma revisão para apresentar o que foi concluído ao cliente, e uma nova sprint é planejada em seguida. Esse ciclo contínuo garante que o produto seja desenvolvido de forma adaptável e em constante alinhamento com as necessidades do cliente. Algumas práticas Scrum usados no desenvolvimento do projeto são:

### <i>Backlog do Produto</i>

O backlog do produto é basicamente uma lista dos requisitos funcionais, chamados de histórias de usuários, e dos requisitos não funcionais. Nessa lista temos aquilo que tem valor para o usuário, e é altamente flexível, podendo ser alterada a qualquer momento. Esse backlog dura até o desenvolvimento final do produto.

O Backlog está disponível à toda equipe e aos PO's no quadro de atividades do Zenhub.

### <i>Planejamento de Sprint</i>

A cada começo de sprint, a equipe, juntamente dos PO's, entram em acordo sobre os itens do backlog a serem realizados nesse ciclo. Os Product Owners escolhem e priorizam os requisitos, onde a equipe define a velocidade de produção, estimada em pontos por história, e também detalham cada história em tarefa e estimam a duração delas.

### <i>Backlog da Sprint</i>

O Backlog da Sprint é gerado após a Sprint Planning, onde itens do backlog do produto são escolhidos para serem realizados nesse ciclo. A equipe organiza como será realizado cada item, podendo alterar quem e como desejam realizar cada tarefa, no entanto, sempre tendo em foco o objetivo da Sprint.

Esse Backlog é escolhido pelos PO's, juntamente com a equipe, a cada início de sprint, destacando, juntamente com os critérios de aceitação, quais itens do Backlog do produto serão realizados.

### <i>Sprint Review</i>

Ao final da Sprint, a equipe demonstra aos P.O's aquilo que foi realizado durante toda a sprint, além de disponibilizar uma versão do produto. Assim, a equipe recebe um feedback de cada história, decidida se estas foram aceitas ou se necessitam voltar ao backlog do Produto. Somente as histórias concluídas por completo poderão ser aceitas.

### <i>Retrospectiva da Sprint</i>

A retrospectiva da Sprint é o último artefato de cada Sprint. A equipe Scrum realiza uma reunião e avalia o processo de desenvolvimento, com o objetivo principal de obter oportunidades de melhoria e debater sobre aquilo que funcionou e sobre aquilo que pode ser melhorado na próxima sprint.

## Kanban

O sistema Kanban propõe uma abordagem com o uso de cartões sinalizadores, chamados de Kanban. Esses devem trazer visibilidade, cadência contínua do fluxo de trabalho e limitação do trabalho. Cada cartão traz informações do trabalho a ser realizado, sendo geralmente os requisitos e pequenas tarefas para a realização deste. Os cartões devem ficar em um ambiente com total visibilidade, tanto ao time, quanto aos P.O 's, por isso eles são alocados em quadros Kanban.

Neste projeto, o quadro Kanban utilizado é uma função do Software Zenhub, onde a equipe, juntamente dos PO 's, utilizam o quadro de tarefas (Board), onde temos diversos cartões sinalizadores. Dentro desse quadro, cada cartão está dividido com suas tarefas, além de estarem em uma listas específicas, onde indicam a finalidade desses. Por exemplo, temos os cartões que podem estar no backlog do produto ou então no backlog da issue, quando algum membro começa a realizar essa tarefa, além de no cartão conter a informação de qual membro está realizando-a, movemos o cartão para a lista "In Progress", e quando totalmente finalizado, ele será movido a lista de "Done". Assim, tanto quanto os membros da equipe, quanto os PO 's, poderão a qualquer momento verificar como está o andamento do projeto como um todo.
