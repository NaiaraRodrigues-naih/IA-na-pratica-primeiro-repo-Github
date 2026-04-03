# Como um LLM Funciona?

## KENSEI CYBERSECURITY ACADEMY — Semana 01

---

## Primeiro: O que e um LLM?

**LLM** = **L**arge **L**anguage **M**odel
(em portugues: *Modelo de Linguagem Grande*)

Sao as IAs que conversam com voce em texto, como o ChatGPT, o Copiloto e o Claude.

Mas como elas sabem responder tudo isso?
Vem entender o processo por dentro!

---

## Etapa 1 — Treinamento

### A fase em que a IA "leu o mundo"

```
Internet + Livros + Codigo + Artigos
           =
     Bilhoes de textos
           =
      IA aprende padroes
```

Imagine uma crianca que leu **todos os livros do mundo**, assistiu **todos os filmes** e leu **todos os sites da internet** antes de falar com voce.

E exatamente isso que acontece no treinamento:
- A IA consome bilhoes de textos
- Ela nao memoriza palavra por palavra
- Ela aprende **padroes** — quais palavras costumam aparecer juntas, o que faz sentido depois do que

> Exemplo de padrao aprendido:
> "Bom..." → provavelmente vem "dia", "tarde" ou "noite"
> "A capital do Brasil e..." → provavelmente vem "Brasilia"

---

## Etapa 2 — Tokenizacao

### A IA nao le letras — ela le pedacos!

Antes de processar qualquer texto, a IA quebra as palavras em **tokens**.

**Token** = um pedaco de palavra (pode ser uma silaba, uma palavra inteira ou ate um simbolo)

```
Sua frase:
"Olá, como vai você?"

Tokens gerados:
["Ol", "á", ",", " como", " vai", " você", "?"]
```

Por que fazer isso?

Porque computadores so entendem **numeros**, nao letras!
Cada token vira um numero:

```
"Ol"   →  1523
"á"    →  890
","    →  11
" como" →  4782
...
```

A IA trabalha com esses numeros o tempo todo.

---

## Etapa 3 — Self-Attention

### A IA presta atencao no contexto

Esta e a parte mais inteligente!

Quando a IA esta processando uma palavra, ela nao olha so para aquela palavra — ela olha para **todas as outras palavras da frase** e calcula: *"qual delas e mais importante para entender essa aqui?"*

Isso se chama **Self-Attention** (auto-atencao).

**Exemplo pratico:**

```
Frase: "O banco estava cheio de gente no domingo."

Quando a IA processa a palavra "banco":
  → olha para "cheio de gente" → nota que ha pessoas
  → olha para "domingo"        → nota que e dia de semana
  → conclusao: "banco" aqui = banco financeiro (nao banco de praca)
```

Sem o self-attention, a IA poderia confundir o significado.
**Com o self-attention, ela entende o contexto completo.**

```
Alta atencao:           "banco" ←→ "gente", "domingo"
Baixa atencao:          "banco" ←→ "o", "estava", "de"
```

---

## Etapa 4 — Geracao

### Como a resposta e montada — palavra por palavra

A IA nao escreve a resposta de uma vez so.
Ela escreve **um token de cada vez**, como uma pessoa digitando devagar.

```
Voce pergunta: "Qual e a capital do Brasil?"

IA pensa:
  proximo token mais provavel → "A"
  proximo token mais provavel → " capital"
  proximo token mais provavel → " do"
  proximo token mais provavel → " Brasil"
  proximo token mais provavel → " e"
  proximo token mais provavel → " Brasilia"
  proximo token mais provavel → "."

Resultado: "A capital do Brasil e Brasilia."
```

Ela repete esse processo ate a resposta estar completa.

> Por isso respostas longas demoram mais — a IA esta gerando token por token!

---

## Resumo Visual do Processo Completo

```
Voce digita uma pergunta
         |
         v
  [ TOKENIZACAO ]
  Texto vira numeros (tokens)
         |
         v
  [ SELF-ATTENTION ]
  IA analisa o contexto de cada token
  e entende o que voce realmente quis dizer
         |
         v
  [ GERACAO ]
  IA preve o proximo token mais provavel
  Repete ate completar a resposta
         |
         v
  Tokens viram texto de novo
         |
         v
  Voce recebe a resposta!
```

---

## Analogia Final: A Cozinheira Experiente

Pense em um LLM como uma **cozinheira que ja fez milhares de receitas**:

| Cozinheira | LLM |
|-----------|-----|
| Aprendeu receitas ao longo da vida | Treinamento com bilhoes de textos |
| Pica os ingredientes em pedacos | Tokenizacao |
| Prova e ajusta conforme o prato | Self-Attention (contexto) |
| Serve o prato prato passo a passo | Geracao token por token |

Ela nao inventa do nada — ela usa tudo que aprendeu para criar algo novo que faz sentido!

---

## O que a IA NAO faz

```
❌ Nao acessa a internet em tempo real (a menos que tenha ferramenta para isso)
❌ Nao tem consciencia nem sentimentos
❌ Nao "sabe" a verdade — ela preve o que e mais provavel
❌ Nao memoriza suas conversas entre sessoes diferentes
```

---

## Sobre

**Curso:** Python do Zero com Copiloto IA
**Academia:** Kensei Cybersecurity Academy
**Autora:** Naiara Rodrigues

> Entender como a IA funciona e o primeiro passo para usa-la com inteligencia!
