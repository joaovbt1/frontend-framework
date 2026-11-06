
## Framework de skills de frontend

| Skill | Quando usar | Comando de instalação (README oficial) |
|---|---|---|
| `design-taste-frontend` ([Leonxlnx/taste-skill](https://github.com/Leonxlnx/taste-skill)) | Definir a direção visual e criar páginas/componentes sem visual genérico | `npx skills add https://github.com/Leonxlnx/taste-skill --skill "design-taste-frontend"` |
| skills do [emilkowalski/skills](https://github.com/emilkowalski/skills) (17: `emil-design-eng`, `animate`, `review-animations`, `break-ui`, `mobile-native`, etc.) | Refinar detalhes e acabamento: animação, polimento, casos extremos | `npx skills@latest add emilkowalski/skills` |
| `impeccable` ([pbakaus/impeccable](https://github.com/pbakaus/impeccable)) | Auditar e criticar UI já feita: `/impeccable audit`, `/impeccable critique` | `npx impeccable install` (flags: `--providers=claude --scope=project\|global`) |

Ordem sugerida: taste para direção, emilkowalski para detalhes, impeccable para auditoria final.

Para verificar e instalar sob demanda, use o comando `/frontend-framework [project|global]`.

Quando a tarefa envolver UI, landing page, redesign ou revisão visual, verifique se as skills estão instaladas. Se alguma que a tarefa pedir estiver faltando, pare e me pergunte se quero instalar, mostrando o comando. Nunca instale sem minha confirmação.

Regras fixas:
- Nunca altere arquivos nem instale nada por conta própria. Mudanças em qualquer projeto só acontecem quando eu pedir ou permitir explicitamente.
- No repositório ms-webpage: por padrão, só leitura, auditoria e crítica. Qualquer alteração ou instalação lá exige pedido meu explícito naquele momento.
- impeccable: usar sem o hook automático. Não rodar `init`, `document` nem `live` sem pedido meu (`live` pode executar `claude`/`codex` com permissões desligadas).
