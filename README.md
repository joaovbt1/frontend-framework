# frontend-framework

Framework de skills de frontend/design para usar projeto a projeto, sempre sob demanda.

| Skill | Uso |
|---|---|
| `design-taste-frontend` ([taste-skill](https://github.com/Leonxlnx/taste-skill)) | Direção visual e criação sem visual genérico |
| [emilkowalski/skills](https://github.com/emilkowalski/skills) | Detalhes e acabamento (animação, polimento) |
| `impeccable` ([impeccable](https://github.com/pbakaus/impeccable)) | Auditoria e crítica (`/impeccable audit`, `/impeccable critique`) |

## Uso

1. Uma vez, instale o comando:
   ```bash
   mkdir -p ~/.claude/commands && cp commands/frontend-framework.md ~/.claude/commands/
   ```
2. (Opcional) Adicione as regras ao seu `~/.claude/CLAUDE.md`:
   ```bash
   cat CLAUDE.section.md >> ~/.claude/CLAUDE.md
   ```
3. Em cada projeto, rode `/frontend-framework` (ou `/frontend-framework global`). Ele verifica o que falta, mostra os comandos e só instala com a sua confirmação.
