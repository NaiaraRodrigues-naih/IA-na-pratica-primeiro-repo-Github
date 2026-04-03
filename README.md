# IA na Prática + Primeiro Repositório no GitHub

## Semana 01 — KENSEI CYBERSECURITY ACADEMY

---

## O que é este repositório?

Este é o meu **primeiro repositório no GitHub!**
Criado durante o curso **Python do Zero com Copiloto IA** da **Kensei Cybersecurity Academy**.

Aqui aprendi a usar a IA como copiloto para estudar programação e a salvar meu progresso no GitHub.

---

## O que é o GitHub?

Imagine o GitHub como uma **nuvem para código**.

```
Seu computador  →  git commit  →  GitHub (nuvem)
    (local)                        (remoto)
```

- Guarda o historico de tudo que voce mudou no codigo
- Voce nunca perde seu trabalho
- Qualquer pessoa (ou voce mesma, de outro computador) pode acessar

---

## Conceitos aprendidos na Semana 01

### O que e IA como Copiloto?

A IA (Inteligencia Artificial) age como um **assistente ao lado**:
- Voce pilota (decide o que fazer)
- A IA copilota (te ajuda a executar)

Nao e trapacar — e usar uma ferramenta poderosa com inteligencia!

---

## Como fazer um Commit — Passo a Passo

Um **commit** e como tirar uma **foto do seu codigo** naquele momento.
Se algo der errado no futuro, voce pode voltar para essa foto!

### No VS Code (jeito mais facil):

```
1. Salve o arquivo         →  Ctrl + S
2. Clique no icone Git     →  barra lateral esquerda (icone de ramal)
3. Clique em +             →  para adicionar (stage) os arquivos
4. Escreva uma mensagem    →  ex: "semana 01 - primeiro commit"
5. Clique em Commit        →  tira a foto!
6. Clique em Sync Changes  →  envia para o GitHub
```

### No terminal (linha de comando):

```bash
# 1. Ver o que mudou
git status

# 2. Adicionar os arquivos
git add nome-do-arquivo.py
# ou adicionar tudo de uma vez:
git add .

# 3. Fazer o commit (tirar a foto)
git commit -m "semana 01 - primeiro commit"

# 4. Enviar para o GitHub
git push
```

---

## Dica de Ouro

> **Faca commits pequenos e frequentes!**
>
> Nao espere terminar tudo para salvar.
> Fez uma parte? Commit.
> Fez outra parte? Commit.
>
> Cada commit e um **checkpoint** — como salvar o jogo!

```
Fez um script?   →  commit
Corrigiu um erro? →  commit
Terminou um desafio? →  commit
```

---

## Como conectar seu repositorio local ao GitHub

```bash
# 1. Inicializar o git na pasta
git init

# 2. Conectar ao repositorio remoto
git remote add origin https://github.com/seu-usuario/nome-do-repo.git

# 3. Definir o branch principal
git branch -M main

# 4. Enviar pela primeira vez
git push -u origin main
```

---

## Estrutura do Repositorio

```
IA-na-pratica-primeiro-repo-Github/
  README.md         ← este arquivo explicativo
```

---

## Sobre

**Curso:** Python do Zero com Copiloto IA
**Academia:** Kensei Cybersecurity Academy
**Autora:** Naiara Rodrigues

> Futura desenvolvedora 
