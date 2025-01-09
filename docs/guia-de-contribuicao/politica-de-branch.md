# Política de _branches_

## Versão

| **Título**        | **Alterações Feitas**                         | **Autor**  | **Data de Hoje**       |
|-------------------|-----------------------------------------------| -----------| ---------------        |
| politica de branch   | Criação do documento de política de branch     | Mateus Maia | 07 de dezembro de 2024 |
## Política de _branches_


Segue-se o fluxo de trabalho descrito pelo [Gitflow](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow), representado pelo diagrama abaixo:


Dessa forma, existem as seguintes categorias de _branches_:

## *_main_*
_Branch_ de produção, com a versão estável mais atual do projeto. Bloqueada para commits e pushs, pode ser interagida apenas através de _pull requests_ provenientes da [_devel_](#devel), [_hotfix branches_](#hotfix-branches) ou [_release branches_](#release-branches).

## *_devel_*
_Branch de desenvolvimento_, agrupa o trabalho de outras _branches_ com o objetivo de se criar uma versão de _release_ para ser submetida à master. Também é bloqueada para commits e pushs, devendo ser modficada através de _pull requests_ provenientes das [_feature branches_](#feature-branches).

## *_Feature Branches_*
_Branches_ criadas a partir da _devel_, para o desenvolvimento de uma funcionalidade específica. Idealmente, uma _feature branch_ deve ser referente à uma issue cadastrada no repositório, para melhor acompanhamento e rastreamento do projeto. Ao final do desenvolvimento, deve-se submeter um _pull request_ visando a _devel_. Se as modificações forem aceitas com sucesso, a _branch_ deve ser apagada.
  #### *Nomenclatura*
  _Feature Branches_ devem seguir o padrão `x_nome_da_issue`, com x sendo o número da _issue_ correspondente no repositório.
  
## *_Hotfix Branches_*
_Branches_ criadas a partir da _master_, para a correção rápida de bugs em produção. Ao final, as atualizações submetidas devem ser integradas tanto à _master_ quanto à _devel_.
  #### *Nomenclatura*
  _Hotfix Branches_ devem seguir o padrão `hotfix_x_nome_da_issue`, com x sendo o número da _issue_ que identifica o bug a ser corrigido.
  
## *_Release Branches_* 
_Branches_ criadas a partir da _devel_, servem para a preparação de uma _release_ do projeto. Deve conter tarefas apenas relacionadas a essa _release_, como correção de bugs ou refino de alguma funcionalidade já implementada. Funcionalidades novas **não** devem ser desenvolvidas nessa _branch_. Com a _release_ preparada, deve-se integrar a branch à master.
  #### *Nomenclatura*
  _Release Branches_ devem seguir o padrão `release/numero_de_versao`, identificando a versão do produto que será entregue naquela _release_.
  
## Mantendo _branches_ atualizadas
Para um fluxo de trabalho sem grandes inconvenientes, recomenda-se manter as _branches_ pessoais de desenvolvimento (features, hotfixes) sempre atualizadas. Antes de se submeter um _pull request_, deve se garantir que a _branch_ possui todas as alterações mais recentes de sua _branch_ de origem. Para isso, deve se utilizar os seguintes comandos:
```
git checkout branch_de_trabalho

git pull branch_de_origem # devel para features, master para hotfixes

git push origin branch_de_trabalho
```