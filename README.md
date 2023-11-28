# Git / Github

> Configurações úteis sobre Git e Github

## Ajustes e melhorias

⚠️ O projeto em desenvolvimento

---


## 🚀 Configuração inicial do GIT

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
git log --decorate
git log --author="Tayse Rosa"
git log shortlog
git shortlog -sn
git log --graph

git show [hash]
```

## ☕ Comandos importantes (Visualizando Diff)
```
git diff
git diff --name-only
```



---

## ☕ Inicializando um repositório
Na pasta do projeto:
```
git status

git init
git add --all
git commit -m "First commit"

```

## 📫 Contribuindo para Bateria JS

Para contribuir com Bateria JS, siga estas etapas:

1. Bifurque este repositório.
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

Copyright :copyright: 2023 · Feito com por ❤️ Tayse Rosa · JS Drums
