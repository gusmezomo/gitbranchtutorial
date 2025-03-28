# Git - Resumo de Aprendizado

Este repositório foi usado para aprender e praticar os principais comandos e fluxos de trabalho do **Git e GitHub**.

Abaixo está um resumo dos conceitos estudados e comandos utilizados, com exemplos reais testados neste projeto.

---

## ✨ Comandos e Conceitos Aprendidos

### 1. `git init`, `git add`, `git commit`
- Inicialização de repositório local
- Adição e commit de arquivos

```bash
git init
git add .
git commit -m "Primeiro commit"
```

---

### 2. Branches
- Criação e troca de branches

```bash
git branch nome-da-branch      # cria uma branch
git switch nome-da-branch      # troca para a branch
git switch -c nova-branch      # cria e troca
```

---

### 3. Merge (junção de branches)
```bash
git switch main
git merge nome-da-branch
```
> Inclui resolução de conflitos com VSCode

---

### 4. Rebase (reescreve o histórico)
```bash
git switch minha-feature
git rebase main
```
> Usado para manter o histórico linear e limpo

---

### 5. Reset (voltar no tempo)
```bash
git reset --soft HEAD~1      # volta, mas mantém arquivos
git reset --mixed HEAD~1     # volta e tira do staging
git reset --hard HEAD~1      # volta e apaga tudo
```

---

### 6. Reflog (histórico secreto do Git)
```bash
git reflog                   # mostra tudo que o HEAD fez
git switch -c recuperado <hash>  # recria branch perdida
```
> Usado para recuperar commits "perdidos"

---

### 7. Restaurar arquivos
```bash
git restore nome.txt              # desfaz mudanças locais
git restore --staged nome.txt    # remove do staging
```

---

### 8. Remover branches
```bash
git branch -d nome     # remove local
git branch -D nome     # remove forçado

git push origin --delete nome  # remove do GitHub
```

---

### 9. Push para GitHub
```bash
git remote add origin https://github.com/seu-usuario/repositorio.git
git push -u origin main
```

---

### 10. Pull Request
- Criado pelo GitHub com botão "Compare & pull request"
- Revisado, mesclado e branch deletada

---

## 🌍 Visualização
Este repositório inclui exemplos visuais (prints) do processo completo:
- Criação de commits
- Branches paralelas
- Conflitos e resolução
- Uso do reflog para recuperação
- Merge e rebase
- Fluxo completo de Pull Request

(*Adicionar imagens na pasta `img/` e referenciar aqui usando `![descricao](img/nome.png)`*)

---

## 🎓 Objetivo
Este repositório foi usado como ambiente de aprendizagem prática do Git e GitHub.
Todos os comandos foram testados e documentados.

---

**Autor:** [gusmezomo](https://github.com/gusmezomo)

