# minhas-skills

As minhas skills para o Claude Code, num só sítio. Funcionam em sessões locais e em Cloud Sessions.

## Usar num projeto

Cria `.claude/settings.json` na raiz do projeto:

```json
{
  "extraKnownMarketplaces": {
    "minhas-skills": { "source": { "source": "github", "repo": "apoli29/minhas-skills" } },
    "impeccable": { "source": { "source": "github", "repo": "pbakaus/impeccable" } }
  },
  "enabledPlugins": {
    "minhas-skills@minhas-skills": true,
    "impeccable@impeccable": true
  }
}
```

O `impeccable` (design: `/impeccable polish`, `/impeccable animate`, …) vem diretamente do repositório original, para receber atualizações.

## Adicionar uma skill

1. Cria `skills/<nome>/SKILL.md`.
2. Sobe a `version` em `.claude-plugin/plugin.json` e em `.claude-plugin/marketplace.json`.
3. Commit e push. Os projetos recebem a skill na próxima sessão.

## Skills

| Skill | Origem | Licença |
|---|---|---|
| `find-skills` | [vercel-labs/skills](https://github.com/vercel-labs/skills) | MIT (`skills/find-skills/LICENSE`) |
