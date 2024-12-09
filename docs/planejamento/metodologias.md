# Metodologias

## Versão 

| **Título**        | **Alterações Feitas**                         | **Autor**  | **Data de Hoje**       |
|-------------------|-----------------------------------------------| -----------| ---------------        |
| Metodologias      | Abertura de documento                         | Bruno Cruz | 07 de dezembro de 2024 |

## Introdução

As **metodologias** utilizadas durante todo o processo do desenvolvimento do projeto Livro Livro serão descritas neste documento. Essas metodologias foram usadas para auxiliar esse desenvolvimento, essas podem ser ditas como metodologias ágeis, com objetivo de ciclos de entrega rápidos, contínuos e incrementais, tais como Lean Inception, XP e Scrum.

## Lean Inception

O Lean Inception é uma metodologia colaborativa usada para alinhar equipes e stakeholders na definição de um Mínimo Produto Viável (MVP) de um produto ou serviço. Ela combina práticas do Lean Startup e do Design Thinking para garantir que o produto inicial entregue ao mercado seja viável, útil e alinhado às necessidades dos usuários e do negócio.

## XP​
O método XP (Extreme Programming) descreve um método voltado principalmente para o desenvolvimento de Software, onde neste há um conjunto de práticas de programação. E o objetivo principal do XP é levar ao extremo esse conjunto de práticas, que são ditas como boas na engenharia de software. Algumas dessas usadas no desenvolvimento do Livro Livre são:

### <i>Programação em Par​</i>

A programação em par é feita de modo em que dois programadores desenvolvem uma mesma parte do código em conjunto, no mesmo ambiente. Isso garante com que ambos possam ter o aprendizado sobre cada elemento realizado no projeto, minimizando a dependência de um único colaborador. Também favorece o nivelamento técnico e o compartilhamento de conhecimento em ambos programadores.

### <i>Testes de aceitação​​</i>

O Desenvolvimento Orientado a Testes (Test Driven Development), o TDD, é amplamente utilizado. Ele garante que cada parte do código criada seja testada unitariamente, minimizando os erros do produto.

### <i>Cliente Presente​​</i>

O cliente é participativo no processo do desenvolvimento do Produto, sempre está em contato com os desenvolvedores, observando o processo e recebendo os resultados de cada processo constantemente.

### <i>Código Coletivo​​</i>

O código fonte é disponibilizado a todos e todos têm acesso e direito para realizar mudanças. Assim, toda a equipe de desenvolvedores pode conhecer todas as partes do produto.

### <i>Padronização de código​​</i>

O código fonte é padronizado com regras ditadas pela equipe. Dessa forma o código fica menos confuso e é mais simples caso seja necessário realizar mudanças futuramente.

### <i>Releases Curtos​​</i>

Sempre são liberadas pequenas versões do produto para o cliente, assim ele poderá testar partes do produto à medida em que este é construído e ajudar no processo de validação.


## Scrum

O método Scrum é um método com foco no gerenciamento do projeto, e esse método propõe artefatos que ditam sobre o planejamento e tarefas dos membros da equipe. É um método iterativo e incremental, onde cada artefato tem uma duração bem definida, criando um fluxo contínuo de trabalho durante ciclos. Esses ciclos são conhecidos como Sprints, e cada sprint determina uma iteração, onde essa tem um tempo determinado e ocorrem vários artefatos durante cada sprint, e ao final de cada sprint, uma release (versão do produto) é liberada ao cliente, além de que ao acabar completamente a sprint, é iniciada outra sprint. Alguns dos artefatos usados no desenvolvimento do projeto são:

### <i>Backlog do Produto</i>

O backlog do produto é basicamente uma lista dos requisitos funcionais, chamados de histórias de usuários, e dos requisitos não funcionais. Nessa lista temos aquilo que tem valor para o usuário, e é altamente flexível, podendo ser alterada a qualquer momento. Esse backlog dura até o desenvolvimento final do produto.

### <i>Planejamento de Sprint</i>

A cada começo de sprint, a equipe, juntamente dos PO 's, entram em acordo sobre os itens do backlog a serem realizados nesse ciclo. Os Product Owners escolhem e priorizam os requisitos, onde a equipe define a velocidade de produção, estimada em pontos por história, e também detalham cada história em tarefa e estimam a duração delas.

### <i>Backlog da Sprint</i>

O backlog da Sprint é gerado após a Sprint Planning, onde itens do backlog do produto são escolhidos para serem realizados nesse ciclo. A equipe organiza como será realizado cada item, podendo alterar quem e como desejam realizar cada tarefa, no entanto, sempre tendo em foco o objetivo da sprint

### <i>Daily Meeting</i>

Uma reunião da equipe realizada diariamente, com curto tempo de realização, aproximadamente 15 minutos, com o objetivo de analisar a situação de cada membro e possíveis obstáculos para a conclusão do produto.

### <i>Sprint Review</i>

Ao final da sprint, a equipe demonstra aos P.O's aquilo que foi realizado durante toda a sprint, além de disponibilizar uma versão do produto. Assim, a equipe recebe um feedback de cada história, decidida se estas foram aceitas ou se necessitam voltar ao backlog do Produto. Somente as histórias concluídas por completo poderão ser aceitas.

### <i>Retrospectiva da Sprint</i>

A retrospectiva da Sprint é o último artefato de cada Sprint. A equipe Scrum realiza uma reunião e avalia o processo de desenvolvimento, com o objetivo principal de obter oportunidades de melhoria e debater sobre aquilo que funcionou e sobre aquilo que pode ser melhorado na próxima sprint.

## Kanban

O sistema Kanban propõe uma abordagem com o uso de cartões sinalizadores, chamados de Kanban. Esses devem trazer visibilidade, cadência contínua do fluxo de trabalho e limitação do trabalho. Cada cartão traz informações do trabalho a ser realizado, geralmente sendo os requisitos e pequenas tarefas para a realização deste. Os cartões devem ficar em um ambiente com total visibilidade, tanto ao time, quanto aos P.O 's, por isso eles são alocados em quadros Kanban.

Neste projeto, o quadro Kanban utilizado é uma função do Software Zenhub, onde a equipe, juntamente dos PO 's, utilizam o quadro de tarefas (Board), onde temos diversos cartões sinalizadores. Dentro desse quadro, cada cartão está dividido com suas tarefas, além de estarem em uma listas específicas, onde indicam a finalidade desses. Por exemplo, temos os cartões que podem estar no backlog do produto ou então no backlog da issue, quando algum membro começa a realizar essa tarefa, além de no cartão conter a informação de qual membro está realizando-a, movemos o cartão para a lista "In Progress", e quando totalmente finalizado, ele será movido a lista de "Done". Assim, tanto quanto os membros da equipe, quanto os PO 's, poderão a qualquer momento verificar como está o andamento do projeto como um todo.

## PMBOK
O PMBOK (Project Management Body of Knowledge) é um guia de boas práticas em gerenciamento de projetos, desenvolvido pelo PMI (Project Management Institute). Ele oferece um conjunto abrangente de diretrizes e terminologias para o gerenciamento efetivo de projetos em diferentes setores e indústrias.
A metodologia do PMBOK se baseia em cinco grupos de processos e dez áreas de conhecimento. Os cinco grupos de processos são:

1. Iniciação: Envolve a definição e autorização do projeto ou fase.
2. Planejamento: Desenvolve o plano do projeto e define os objetivos e as atividades necessárias.
3. Execução: Concentra-se na coordenação de pessoas e recursos para executar o plano do projeto.
4. Monitoramento e Controle: Acompanha, revisa e regula o progresso e o desempenho do projeto.
5. Encerramento: Formaliza a aceitação do projeto e garante a conclusão adequada de todas as atividades.

As dez áreas de conhecimento do PMBOK incluem integração, escopo, tempo, custo, qualidade, recursos humanos, comunicação, riscos, aquisições e partes interessadas.