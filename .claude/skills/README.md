# Скилы команды PlanVIA

Скилы — инструкции, которые Claude Code подхватывает автоматически, когда задача совпадает с их описанием. Роли из `.claude/agents/` получают свои скилы через поле `skills:` (они загружаются при старте) и через список «Скилы роли» в теле файла роли.

Перед работой любой маркетинговый скил читает `.claude/product-marketing.md`. Там контекст PlanVIA и правила, которые сильнее советов скилов.

## Кто чем пользуется

| Роль | Загружаются сразу | По необходимости |
|---|---|---|
| seo-researcher | ai-seo, content-strategy, competitors | seo-audit, programmatic-seo, schema |
| writer | copywriting, copy-editing | ai-seo, schema, competitors |
| social-producer | social, video | image |
| community-scout | social (раздел listening) | — |
| outreach | influencer-marketing, cold-email | link-building, public-relations, directory-submissions |
| analyst | analytics | ai-seo (замер AI-видимости) |
| developer | using-n8n-skills-official, supabase | остальные `n8n-*-official`, n8n-self-hosting, supabase-postgres-best-practices, schema, analytics |
| fact-checker, alerts-monitor | — | — |

## Источники

Скопированы без изменений, кроме удалённых папок `evals/`. Скрипты из скилов не запускались при установке.

| Скилы | Источник | Коммит | Лицензия |
|---|---|---|---|
| ai-seo, analytics, cold-email, competitors, content-strategy, copy-editing, copywriting, directory-submissions, image, influencer-marketing, link-building, programmatic-seo, public-relations, schema, seo-audit, social, video | [coreyhaines31/marketingskills](https://github.com/coreyhaines31/marketingskills) | 88c79f6 | MIT, © 2025 Corey Haines |
| `*-official` (13 скилов n8n) | [n8n-io/skills](https://github.com/n8n-io/skills) — официальные, под MCP n8n | 27b6b9f | Apache 2.0, © n8n GmbH |
| n8n-self-hosting | [czlonkowski/n8n-skills](https://github.com/czlonkowski/n8n-skills) | e037563 | MIT, © 2025 Romuald Członkowski |
| supabase, supabase-postgres-best-practices | [supabase/agent-skills](https://github.com/supabase/agent-skills) | c9be0e9 | MIT, © 2026 Supabase |

Обновить: склонировать источник, заменить папку скила, удалить `evals/`, просмотреть изменения в PR.
