# Manipulação de repositórios

Repositórios podem ser manipulados através de interfaces de linha de comando.

## _Placeholders_

Em blocos de código, colchetes são utilizados para indicar _placeholders_.

```
git comando [placeholder]
```

## Comandos

- [Comando _add_](#comando-add)
- [Comando _branch_](#comando-branch)
- [Comando _checkout_](#comando-checkout)
- [Comando _clone_](#comando-clone)
- [Comando _commit_](#comando-commit)
- [Comando _config_](#comando-config)
- [Comando _help_](#comando-help)
- [Comando _init_](#comando-init)
- [Comando _log_](#comando-log)
- [Comando _merge_](#comando-merge)
- [Comando _pull_](#comando-pull)
- [Comando _push_](#comando-push)
- [Comando _remote_](#comando-remote)
- [Comando _restore_](#comando-restore)
- [Comando _revert_](#comando-revert)
- [Comando _show_](#comando-show)
- [Comando _status_](#comando-status)

### Comando _add_

Comando _add_ modifica o estado de um ou mais arquivos para _staged_.

```
git add [arquivo]
```

### Comando _branch_

Comando _branch_ exibe a lista de _branches_ do repositório ou cria uma nova com o nome especificado.

```
git branch

git branch [branch]
```

Comando _branch_ com _-d_ remove a _branch_ especificada se ela não possuir diferenças com a _branch_ _master_.

```
git branch -d [branch]
```

Comando _branch_ com _-D_ remove a _branch_ especificada.

```
git branch -D [branch]
```

Comando _branch_ com _--merged_ exibe as _branches_ que estão mescladas com a atual.

```
git branch --merged
```

Comando _branch_ com _--no-merged_ exibe as _branches_ que não estão mescladas com a atual.

```
git branch --no-merged
```

### Comando _checkout_

Comando _checkout_ muda o repositório para a _branch_ especificada.

```
git checkout [branch]
```

Comando _checkout_ modifica o conteúdo e estado de um ou mais arquivos _modified_ para o estado _unmodified_.

```
git checkout [arquivo]
```

### Comando _clone_

Comando _clone_ baixa um repositório remoto.

```
git clone [repositório remoto]
```

### Comando _commit_

Comando _commit_ salva os arquivos _staged_ em um novo _commit_ do repositório.

```
git commit -m "[mensagem]"
```

Comando _commit_ com _--amend_ salva os arquivos _staged_ no último _commit_ do repositório.

```
git commit --amend

git commit --amend -m "[mensagem]"

git commit --amend --no-edit
```

Comando _commit_ com _-a_ ou -_am_ salva todos os arquivos _modified_ em um novo _commit_ do repositório.

```
git commit -a -m "[mensagem]"
git commit -am "[mensagem]"
```

### Comando _config_

Comando _config_ modifica ou acessa variáveis locais ou globais.

Comando _config_ com _--global_ _user.name_ modifica o valor da variável global que referencia o nome do usuário.

```
git config --global user.name "[nome]"
```

Comando _config_ com _--global_ _user.email_ modifica o valor da variável global que referencia o _e-mail_ do usuário.

```
git config --global user.email "[e-mail]"
```

Comando _config_ com _--list_ exibe uma lista de variáveis configuradas.

```
git config --list
```

### Comando _help_

Comando _help_ exibe informações sobre o Git.

```
git help
```

Comando _help_ exibe informações sobre o comando especificado.

```
git help [comando]
```

### Comando _init_

Comando _init_ inicia um repositório no diretório.

```
git init
```

### Comando _log_

Comando _log_ exibe informações sobre os _commits_ do repositório.

```
git log
```

Comando _log_ com _--oneline_ exibe informações sobre os _commits_ do repositório em uma linha cada.

```
git log --oneline
```

### Comando _merge_

Comando _merge_ mescla a _branch_ atual com a especificada.

```
git merge [branch]
```

### Comando _pull_

Comando _pull_ baixa as versões de uma _branch_ de um repositório remoto.

```
git pull [repositório remoto] [branch]
```

### Comando _push_

Comando _push_ envia as versões do repositório local para uma _branch_ de um repositório remoto.

```
git push [repositório remoto] [branch]
```

### Comando _remote_

Comando _remote_ com _add_ adiciona um nome para referenciar um repositório remoto.

```
git remote add [repositório remoto] [URL repositório remoto]
```

Comando _remote_ com _-v_ exibe uma lista dos repositórios remotos salvos.

```
git remote -v
```

### Comando _restore_

Comando _restore_ retorna um ou mais arquivos _modified_ ou _deleted_ para o estado _unmodified_.

```
git restore [arquivo]
```

Comando _restore_ com _--staged_ retorna um ou mais arquivos _staged_ para seu estado anterior.

```
git restore --staged [arquivo]
```

### Comando _revert_

Comando _revert_ retorna a versão do repositório para a do _commit_ especificado.

Essa reversão criará um novo _commit_ e não apagará os anteriores.

```
git revert [commit]
```

### Comando _show_

Comando _show_ exibe informações sobre o último _commit_ ou um outro especificado.

```
git show
git show [commit]
```

### Comando _status_

Comando _status_ exibe o estado do repositório no momento dComando.

```
git status
```

Comando _status_ com _--short_ ou _s_ exibe o estado do repositório no momento do comando e de forma simplificada.

```
git status --short
git status -s
```
