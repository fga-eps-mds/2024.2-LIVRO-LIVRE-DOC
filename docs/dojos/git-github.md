# Dojô Git / GitHub

# Versão

| **Título**        | **Alterações Feitas**                         | **Autor**  | **Data de Hoje**       |
|-------------------|-----------------------------------------------| -----------| ---------------        |
| Dojo Git/GitFlow    | Subindo documento versão 1                    | Mateus Maia | 09 de dezembro de 2024 |

## Introdução

### Git
Git é um **sistema de controle de versão distribuído** usado para rastrear alterações no código fonte durante o desenvolvimento de software.
- Permite que vários desenvolvedores trabalhem simultaneamente no mesmo projeto
- Audita as alterações feitas em arquivos específicos ao longo do tempo.
- Permite que os desenvolvedores revertam para versões anteriores, criem novas funcionalidades em paralelo e colaborem de maneira eficaz.

### GitHub:
GitHub é uma **plataforma de hospedagem** baseada na web para projetos Git, fornecendo uma interface visual para o controle de versão e colaboração em equipe.

Ele permite que os desenvolvedores hospedem seus repositórios Git remotamente na nuvem e fornece recursos adicionais, como rastreamento de problemas, controle de acesso, integração contínua e muito mais.

## Conceitos chave

### Commit:
Um commit no Git é uma operação na qual as alterações feitas em arquivos específicos são salvas no repositório **local** Git.
- Cada commit é acompanhado de uma mensagem que descreve as alterações feitas, fornecendo contexto sobre o que foi modificado.
- Commits ajudam a rastrear e documentar o progresso do desenvolvimento ao longo do tempo.

### Branch:
Uma branch no Git é uma ramificação independente do código fonte principal (geralmente chamado de branch "master" ou "main").

As branches permitem que os desenvolvedores trabalhem em novas funcionalidades ou correções de bugs sem interferir no código principal.

Depois que as alterações em uma branch são concluídas e testadas, elas podem ser mescladas de volta a branch principal por meio de um processo chamado de "merge".

### Merge:
Merge é o processo de combinar as alterações de uma branch em outra.

Por exemplo, você pode ter uma branch de desenvolvimento onde as novas funcionalidades são adicionadas e, quando estiverem prontas, você pode mesclá-las de volta para a branch principal (master ou main).

### Pull Request (Pedido de Pull):
Um pull request é uma solicitação feita por um colaborador de um repositório Git para incorporar suas alterações em uma branch específica desse repositório.

Geralmente, os pull requests são usados em projetos colaborativos para revisão de código e integração de novas funcionalidades ou correções de bugs. Os mantenedores do projeto podem revisar as alterações propostas, fazer comentários e, eventualmente, mesclar o pull request se estiverem satisfeitos com as alterações.

## Tutorial de COntrinuição Git

Dojo de git do grupo do Livro Livre da disciplina de EPS.

## Criando a sua chave ssh

### 1. Gerando a sua chave SSH

No seu terminal use o comando:

``` ssh-keygen -t rsa -b 4096 -C "seu-email@exemplo.com"```

### 2. Adicionando a sua chave SSH RSA ao ssh-agent

Abra um novo terminal e utilize esse comando:

```eval "$(ssh-agent -s)"```

Em seguida esse comando:

```ssh-add ~/.ssh/id_rsa```

### 3. Adicionar a sua chave SSH ao GitHub

Em um terminal copie a chave SSH pública para a área de transferência, usando esse comando:

```cat .ssh/id_rsa.pub```

No GitHUb acesse 
- Acesse Settings > SSH and GPG keys.
- Clique em New SSH Key.
- Cole a chave pública copiada no campo e salve.

### 4. Testar a conexão SSH

Para verificar se a chave SSH está funcionando, execute:

``` ssh -T git@github.com  ``` 

## Passos a serem executados

### 1. Clone
Clonem esse repositório para suas máquinas utilizando o ssh.  

### 2. Branches

De acordo com nossa política de contribuição, devemos seguir o padrão estipulado de x_nome_da_issue para feature branches e hotfix_x_nome_da_issue para hotfix branches.

#### 2.1 Crie branch de feature
```$ git checkout -b x_nome_da_issue_seu_nome```

### 3. Stage/Add
1. Crie um arquivo .js com nome `feature.js` com o conteúdo do [feature.txt](feature.txt);
2. Salve suas mudanças;
3. Dê "stage" em suas mudanças. ```$ git add feature.js```

### 4. Commit
Commite suas mudanças para sua branch atual seguindo nossa política de commit.
#### 4.1 Commite suas mudanças.
```$ git commit -m "feat: create javascript feature"```

### 5. Push
Envie para o repositório de origem as mudanças feitas.
```$ git push origin x_nome_da_issue_seu_nome```

### 6. Rebase/Merge
1. Edite o arquivo [dojo.py](dojo.py) conforme as instruções;
2. Atualize sua branch com a `main` usando do rebase; ```$ git pull --rebase origin main```
3. Siga os passos conforme as instruções ministradas e sua linha de comando;
4. Atualize a sua branch com as novas mudanças. ```$ git push -f origin x_nome_da_issue_seu_nome```

### 7. Abra um Pull Request para a Main
Siga as instruções dadas em [política de contribuição](https://github.com/fga-eps-mds/EPS-2020-2-G1/blob/main/CONTRIBUTING.md) e seguindo nosso [pull request template](https://github.com/fga-eps-mds/EPS-2020-2-G1/blob/main/.github/pull_request_template.md).