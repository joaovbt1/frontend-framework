---
description: Verifica e (com confirmação) instala o framework de skills de frontend (taste, emilkowalski, impeccable)
argument-hint: "[project|global]  (padrão: project = projeto atual)"
---

Escopo pedido: `$ARGUMENTS` (vazio = `project`, isto é, o diretório atual).

Você vai preparar o framework de skills de frontend. Siga estes passos, nesta ordem, sem pular a confirmação.

## 1. Verificar (somente leitura)
Veja quais destas skills já existem em `./.claude/skills/` (projeto) e `~/.claude/skills/` (global), ou aparecem como skills disponíveis:
- `design-taste-frontend`
- as skills do emilkowalski: emil-design-eng, animate, animate-expo, animation-performance, animation-vocabulary, apple-design, ask-sonner, break-ui, choreograph, find-animation-opportunities, improve-animations, mobile-native, pick-ui-library, prototype, remove-animations, review-animations, write-swift
- `impeccable`

Mostre uma tabela: skill, instalada (sim/não), onde.

## 2. Mostrar os comandos e PERGUNTAR
Para o que estiver faltando, mostre os comandos abaixo e pergunte se pode rodar. **Nunca instale sem a minha confirmação explícita nesta conversa.** Se tudo já estiver instalado, apenas informe e pare.

Escopo `project` (padrão, a partir da raiz do projeto atual):
```bash
npx skills add https://github.com/Leonxlnx/taste-skill --skill "design-taste-frontend" -a claude-code -y
npx skills@latest add emilkowalski/skills -a claude-code -y
npx impeccable install --providers=claude --scope=project
```

Escopo `global`: os mesmos comandos, adicionando `-g` nos dois primeiros e trocando por `--scope=global` no terceiro.

Os comandos do README oficial são:
- `npx skills add https://github.com/Leonxlnx/taste-skill --skill "design-taste-frontend"`
- `npx skills@latest add emilkowalski/skills`
- `npx impeccable install` (flags `--providers` e `--scope` documentadas no README do impeccable)

As flags `-a`, `-y` e `-g` do CLI `skills` NÃO estão nos READMEs: antes de rodar, confirme com `npx skills add --help` e, se alguma flag não existir, me mostre o erro e use o modo interativo em vez de improvisar.

## 3. Regras de instalação
- Instalar apenas no escopo pedido, e em nenhum outro diretório.
- **Hook do impeccable: recusar.** Uso apenas manual. Se o instalador oferecer o hook, responda não.
- Não rodar `/impeccable init`, `document` nem `live` agora. Eles escrevem arquivos e só rodam se eu pedir.
- Se algum comando falhar, mostre o erro e a alternativa. Não improvise.

## 4. Confirmar
Depois de instalar, peça para eu recarregar a sessão e liste os nomes de chamada: `design-taste-frontend`, as skills do emilkowalski pelos nomes acima e `/impeccable <comando>`.
