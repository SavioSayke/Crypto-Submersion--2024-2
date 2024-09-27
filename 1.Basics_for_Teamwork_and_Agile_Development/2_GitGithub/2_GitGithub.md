# Aprenda Git e GitHub em 3 dias

![Git](https://git-scm.com/images/logos/2color-lightbg@2x.png)

## Conceito

**Git** é um sistema de controle de versão distribuido que controla versão dos arquivos (versionamento de arquivos). Como os desenvolvedores fazem alterações no projeto, qualquer versão anterior do projeto pode ser recuperada a qualquer momento.

Os desenvolvedores podem revisar o histórico do projeto para descobrir:

Quais alterações foram feitas?
Quem fez as alterações?
Quando as alterações foram feitas?
Por que as alterações foram necessárias?


## Download

1. Para baixar, acesse o link:
```
https://git-scm.com/downloads
```
2. Basta fazer uma instalação padrão, aceitando os Termos de Uso e Avançando.
3. Depois que finalizar a instalação, procure o programa "Git Bash" no seu computador e abra-o, pois é ele que vamos utilizar para iniciar o Git.

## 1. Primeiros comandos

Recomendo que digite esse primeiro comando para **verificar a versão instalado do Git**
```
git --version
```
Caso precise de ajudar e também mais detalhes dos comandos, digite:
```
git help
```

## 2. Configurando o Git

Nesse momento, você precisará registrar seu **UserName** e **UserEmail** para que outros colaboradores saibam quem é você e tenham o histórico de tudo o que você fez.

Registrar com configurações globais seu UserName:
```
git config --global user.name "DIGITE_SEU_UserName_AQUI"
```

Registrar com configurações globais seu UserEmail:
```
git config --global user.email DIGITE_SEU_UserEmail_AQUI
```

Agora vamos iniciar a branch main:
```
git config --global init.default main
```

## 3. Iniciando seu primeiro repositório

Esteja no diretório com os arquivos que você quer trabalhar: cd /SEU_DIRETORIO
```
git init
```

## 4. Comandos

Para verificar o estado dos seus arquivos:
```
git status
```

Existem os arquivos **Untracked** que são arquivos que ainda não fazem parte do Git. Se houver alguma alteração qualquer nos arquivos, ele **não vai tirar uma *Snapshot*** que é tirar uma cópia e criar uma nova versão dos arquivos enquanto os arquivos estiverem **Untracked**.

Para tornar o(s) arquivo(s) **Tracked**, iremos usar o **add**:
```
git add NOME_DO_ARQUIVO.EXTENSAO
```

Caso queira add **todos os arquivos** do diretório de uma vez, ou seja, torná-los **tracked** e assim criar um *snapshot* de sua versão:
```
git add .
```

Os arquivos *tracked* ficão com o status de **staged** ou seja, ele está pronto para o commit.

**unstaged** ele não está pronto para o commit.

Caso queira remover o arquivo do status de **staged** para **unstaged** e assim ele não participará do Git, digite:
```
git rm --cached NOME_DO_ARQUIVO.EXTENSAO
```

Agora, vamos criar nossa primeira versão, nosso primeiro **commit** desses arquivos com status de **staged**.
```
git commit -m "DIGITE UMA MENSAGEM"
```

Caso tenha alguma alteração nos arquivos, você pode usar o **diff** para visualizar essa alteração:
```
git diff 
```

Se um arquivo foi alterado depois do commit, ele entrará no status **working**, então basta usar o *git add* para mudar o status para **staged** ou seja, pronto para o commit (git commit -m "SUA MENSAGEM"). Criando assim um novo commit, uma nova versão do(s) arquivo(s).
Você pode visualisar os commit's usando:
```
git log
OU
git log --oneline
```

Passar o(s) arquivo(s) do state **working** direto para o **commit**, pulando o status de **staged**
```
git commit -a -m "SUA MENSAGEM"
```

Você pode **remover** seus arquivos utilizando *git rm*. O arquivo será removido, ficará com a tag **deleted** e o status de **staged**. Para restaurar, use o *git restore --staged*
```
git rm NOME_DO_ARQUIVO.EXTENSAO
git restore --staged NOME_DO_ARQUIVO.EXTENSAO
```

Caso você remova o arquivo pelo diretório (sem ser pelo comando do git), você pode usar o *git restore*, puxando a última versão salva dos arquivos.
```
git restore NOME_DO_ARQUIVO.EXTENSAO
```

Renomear um arquivo, ele recebe a tag *renamed* e já fica pronto para o commit:
```
git mv NOME_ATUAL_DO_ARQ.EXT NOME_NOVO_DO_ARQ.EXT
```

Alterar mensagem do último commit adicionado:
```
git commit -m "SUA_NOVA_MENSAGEM" --amend
```

Log detalhado:
```
git log -p
```

git reset

* ```git reset --soft ID_DA_COMMIT```
  * Reseta o commit, mas mantem em **staged** já pronta para um novo commit;
* ```git reset --mixed ID_DA_COMMIT```
  * (É o reset padrão) Reseta o commit, mas muda o estado para **unstaged** sendo necessário adiciona-los novamente;
* ```git reset --hard ID_DA_COMMIT```
  * Reseta o commit e remove todas as alterações feitas após o commit escolhido, não podendo mais recuperar

Alterar um **atalho** do git para um de sua escolha:

```
git config --global alias.SEU_ATALHO "COMANDO_PADRAO"
```

Ex: git config alias.log1 "log --oneline"
Assim, ao digitar *git log1* seria como se você tivesse digitando *git log --oneline* (Caso não tenha espaço como o "log --online", não precisa usar as aspas).

## 5. Branch

É uma ramificação separada, uma cópia da branch principal para que você possa trabalhar com segurança sem afetar a main.

**Criar uma nova Branch**
```
git branch NOME_BRANCH
```

**Mudar a Branch**
```
git switch NOME_BRANCH
OU
git checkout NOME_BRANCH
```

**Apagar a Branch**
```
git branch -d NOME_BRANCH
```

**Fazer o merge da branch com a main**
```
git merge NOME_BRANCH -m "MENSAGEM_DO_MERGE"
```

---

![Github](https://github.blog/wp-content/uploads/2024/07/github-logo.png)

**Github** é um serviço de hospedagem para projetos que utilizam o Git. Ele faz essa sincronização com o Git e armazena seus repositórios na nuvem para que você possa gerenciar projetos, trabalhar de forma colaborativa e manter projetos seus a salvo na nuvem.

**Com esse comando, conseguimos associar o repositório local ao repositório remoto**
```
git remote add origin https://github.com/SEU_USUARIO/SEU_REPOSITORIO.git
```

**Agora, para enviar do repositório local para o repositório do Github**
```
git push -u origin main
```

**Usado para atualizar um repositório local a partir da versão remota**
```
git pull
```

---

*_Issues (Problemas)_*

**Os GitHub Issues são itens que podem ser criados em um repositório para planejar, discutir melhorias, reportar bugs e monitorar o projeto.**

*_Releases (Lançamento)_*
**Releases são versões lançadas do software, quando fazemos uma alteração muito significativa ou muitas mudanças/novidades são introduzidas ao projeto, é interessante criar releases para disponibilizar e categorizar cada versão do software, seu histórico e informando através de tags as versões existentes do projeto .**

---