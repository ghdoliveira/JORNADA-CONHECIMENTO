# Guia rápido de Git — TCC

## Regra do grupo

Cada integrante trabalha na **sua própria branch**.

Exemplo:

* `main` → versão principal do projeto
* `nathan`
* `gustavo`
* `guilherme`
* `leonardo`

---

## 1. Antes de começar a programar

Entre na sua branch e atualize tudo:

```bash
git checkout sua-branch
git pull origin sua-branch
git checkout main
git pull origin main
git checkout sua-branch
git merge main
git push origin sua-branch
```

### Exemplo com Nathan

```bash
git checkout nathan
git pull origin nathan
git checkout main
git pull origin main
git checkout nathan
git merge main
git push origin nathan
```

---

## 2. Depois de programar

Salvar e enviar suas alterações:

```bash
git add .
git commit -m "feat: descrição da alteração"
git push origin sua-branch
```

### Exemplo

```bash
git add .
git commit -m "feat: adiciona tela inicial"
git push origin nathan
```

---

## 3. Quando quiser mandar para a main

Entre na `main`, faça o merge e envie:

```bash
git checkout main
git pull origin main
git merge sua-branch
git push origin main
```

### Exemplo

```bash
git checkout main
git pull origin main
git merge nathan
git push origin main
```

---

## 4. Se der conflito

Abrir o arquivo, corrigir, salvar e rodar:

```bash
git add .
git commit -m "resolve conflito"
git push origin main
```

---

## 5. Comandos principais

### Ver branch atual

```bash
git branch
```

### Trocar de branch

```bash
git checkout nome-da-branch
```

### Ver arquivos alterados

```bash
git status
```

---

## Resumo rápido

### Para começar o trabalho

```bash
git checkout sua-branch
git pull origin sua-branch
git checkout main
git pull origin main
git checkout sua-branch
git merge main
git push origin sua-branch
```

### Para salvar

```bash
git add .
git commit -m "feat: alteração"
git push origin sua-branch
```

### Para mandar para a main

```bash
git checkout main
git pull origin main
git merge sua-branch
git push origin main
```
