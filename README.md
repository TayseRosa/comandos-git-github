# Git / Github

> Configurações úteis sobre Git e Github

---

## 🚀 Inicializando um repositorio (mais utilizado no dia a dia)
Na pasta do projeto:
```
git status

git init
git add --all
git commit -m "First commit"
git remote add origin REMOTE-URL
git push origin main

```


## 🚀 Enviando mudanças para um repositorio (mais utilizado no dia a dia)
Na pasta do projeto:
Para onde: origin
Branch que estou: master
[Enter]
```
git push origin master
```

## ☕ Corrigindo mensagem de commit
```
git commit --amend -m "Teste de novo commit"
git log --oneline
```


## ☕ Configuracao inicial do GIT

```
git config --global user.name "Tayse Rosa"
git config --global user.email "tayse_rosa@yahoo.com.br"
```

## ☕ Configurar editor
```
git config --global core.editor sub
git config --global core.editor vim
git config --global core.editor emacs
git config --global core.editor "code --wait"
```
---

## ☕ Ciclo de vida dos status de seus arquivos
UnTracked (não marcado) - Acabou de ser adicionado no repositório, mas ainda não foi visto pelo Git.

UnModified (não modificado) - Ele existe no GIT mas não teve nenhuma modificação em cima dele.

Modified (Modificado) - Arquivo foi modificado.

Staged - Momento em que a versão for fechada, levara esses arquivos.

---

## ☕ Comandos importantes (Visualizando Logs)
```
git config --list

git log
git log --oneline
git log --decorate
git log --author="Tayse Rosa"
git log shortlog
git shortlog -sn
git log --graph

git show [hash]

git remote -v
```

## ☕ Comandos importantes (Visualizando Diff)
```
git diff
git diff --name-only
```

## ☕ Desfazendo
```
git reset --soft [hash]


git log
git status
git diff

Quando o arquivo NÃO esta na area de staged:
git checkout [nome do arquivo]

Quando o arquivo JÁ esta na area de staged:
git reset HEAD [nome do arquivo]

git reset --soft 
git reset --mixed
git reset --hard
```

ℹ️ git reset - Vai pegar as modificaçoes, voltar o commit, mas o arquivo permanece como staged, com a modificação pronta para ser commitado novamente.

ℹ️ git mixed - Vai pegar as modificaçoes, voltar o commit, vai voltar para antes do staged (unmodified)

ℹ️ git hard - Vai ignorar a existencia deste commit e tudo o que foi feito nele.

---


## ☕ Conectando ao GitHub com SSh
Problemas para subir o código para o repositório remoto?
Temos esse problema porque o Github precisa identificar você de alguma forma, e para isso o Github precisa autenticar um usuário remoto ao servidor atraves do SSH.

SSH é um protocolo que serve para autenticar um usuário remoto ao servidor, é baseado em uma chave pública e uma chave privada, onde apenas a chave privada consegue abrir a chave pública.
Por isso, enviamos a chave pública para o servidor (GitHub) e com a nossa chave privada na nossa máquina conseguimos abrir a chave publica do github e subir o codigo.

1º - Gerar a chave SSH
2º - Adicionar a chave SSH a sua conta GitHub

### Gerar uma nova chave SSH
```
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
```
[x]- Isso cria uma nova chave ssh, utilizando seu próprio email

[x]- [Enter] 3x

Para copiar a sua chave, basta:
```
cd ~/.ssh
ls
cat id_rsa.pub
```
Copia o código

### Adicionar sua chave SSH ao GitHub
No https://github.com: clica na sua foto de perfil > settings > do lado esquerdo tem a opção "SSH and GPG Keys" > Clica em New SSH key.

---

## ☕ O que é um branch?
É um ponteiro móvel que leva a um commit.

### Criando um branch
```
git checkout -b [nome do branch]

git branch
```

### Dando merge em branchs
```
git merge [nome da branch que quer mergir com a atual] 
```

### Deletando um branch
```
git branch -D [nome do branch]
```

## ☕ Criando .gitignore
Fonte de templates de .gitignore: https://github.com/github/gitignore

Criar arquivo .gitignore
```
teste.txt
```

---
## ☕ Criando Alias
```
git config --global alias.s status
```

## ☕ Versionando com tags
```
git tag -a 1.0.0 -m "Readme finalizado"
git push origin master --tags
```
Release modificadas


## ☕ Git revert
```
git revert [hash]
```

## ☕ Apagar tags e branches remoto
```
//tag local
git tag -d 1.0.0 

//tag remoto
git push origin :1.0.0

//branch remoto
git push origin :test
```


---
## 📫 Contribuindo com este repositório

Para contribuir com este repositório, siga estas etapas:

1. Faça um fork deste repositório.
2. Crie um branch: `git checkout -b <nome_branch>`.
3. Faça suas alterações e confirme-as: `git commit -m '<mensagem_commit>'`
4. Envie para o branch original: `git push origin <nome_do_projeto> / <local>`
5. Crie a solicitação de pull.

Como alternativa, consulte a documentação do GitHub em [como criar uma solicitação pull](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request).

## 🤝 Colaboradores

Agradecemos às seguintes pessoas que contribuíram para este projeto:

<table>
  <tr>
    <td align="center">
      <a href="https://github.com/TayseRosa" title="Tayse Code Rosa">
        <img src="https://avatars.githubusercontent.com/u/31596454?v=4" width=115><br>
        <sub>
          <b>Tayse Rosa</b>
        </sub>
      </a>
    </td>
  </tr>
</table>

Copyright :copyright: 2023 · Feito com por ❤️ Tayse Rosa 
