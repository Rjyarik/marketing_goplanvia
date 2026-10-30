# План на 29–30 октября 2026

Цель двух дней: запустить систему и получить первые результаты агентов, которые не зависят от коннекторов. Задачи, которые ждут доступов, начинаются, как только Ярослав их даст.

## Ярослав (около 1,5 часа за два дня)

| # | Что | Время | Зачем |
|---|---|---|---|
| 1 | Claude GitHub App на marketing_goplanvia | 5 мин | Агенты смогут сохранять работу в репозиторий |
| 2 | Опубликовать проект в Lovable, отправить себе ссылку goplanvia.com/plans в Telegram | 10 мин | Проверить превью страниц |
| 3 | Supabase: Site URL `https://goplanvia.com`, Redirect URLs, секрет Google, ключ Apple | 20 мин | Сейчас вход через Google и Apple не работает — теряем регистрации |
| 4 | n8n: включить Instance-level MCP, добавить коннектор на claude.ai | 15 мин | Ролики, Postiz, AI-замер |
| 5 | Коннектор BabyLoveGrowth MCP | 10 мин | Search Console и GA4 для аналитика |
| 6 | Search Console, Bing, Meta: подтвердить goplanvia.com | 15 мин | Индексация и превью в Meta |
| 7 | Ответить: убрать фейковые цифры с /cashback? | 1 мин | |
| 8 | Прочитать черновик спецификации совместной поездки и ответить на вопросы в конце | 15 мин | Главный рубеж плана |

## Координатор

- [x] Заполнить репозиторий: правила, роли, шаблоны, таблицы, backlog.
- [x] Свести расхождения между планом и «Стратегией» в документе.
- [x] Черновик спецификации совместной поездки — `plan/specs/group-trip-mvp.md`.
- [x] Запустить первую волну агентов (ниже) и проверить результаты.
- [x] Отправить работу в GitHub, как только появится доступ.
- [x] Собрать вопросы агентов к Ярославу — `plan/questions.md`.
- [x] 29 октября вечером: итог дня Ярославу и следующая волна задач.

## Агенты: первая волна (29 октября)

| Роль | Задача | Результат |
|---|---|---|
| alerts-monitor | 6–8 первых записей для /travel-alerts: EES, ETIAS, забастовки ноября–декабря, туристические сборы 2027 | `content/alerts/` |
| outreach | 25 статей-подборок «AI trip planner», «group trip planner apps», «Wanderlog alternatives» (EN+ES), которые цитируют поиск и AI, с публичными контактами авторов | `data/outreach-targets.csv` |
| seo-researcher | 3 брифа: хаб /plan/friends-trip-planner (EN), «3 days in Lisbon with friends» (EN), «Semana Santa en Oporto con amigos» (ES) | `research/briefs/` |

## Агенты: вторая волна (30 октября)

| Роль | Задача | Зависит от |
|---|---|---|
| fact-checker | Проверить записи /travel-alerts первой волны | Идёт с 28.10 |
| writer | Текст хаба /group-trip-planner (EN готов как черновик 28.10, 17 пометок «проверить»), затем ES | Ответы из plan/questions.md |
| outreach | Тексты профилей для каталогов AI-инструментов — готово 28.10 | — |
| community-scout | Первый дайджест тредов Reddit и Quora, режим «без ссылок» | — |
| outreach | Первые 25 микрокреаторов ES/EN | — |
| analyst | Базовый AI-замер | Коннектор n8n |
| social-producer | Первые 3 сценария роликов на зимние темы | Коннектор n8n для медиа; сценарии можно раньше |

## 30 октября: что запущено на самом деле

| Поток | Задача | Результат | Статус |
|---|---|---|---|
| fact-checker | Проверить черновик хаба /group-trip-planner (15 пометок) | `reports/fact-checks/2026-10-30-group-trip-planner-hub.md` | doing |
| writer | «3 days in Lisbon with friends» EN, затем «Semana Santa en Oporto con amigos» ES | `content/pages/2026-10-30-*.md` | doing |
| outreach | Креаторы до 25, проверка 8 существующих | `data/creators.csv`, `content/outreach/2026-10-30-creators-report.md` | doing |
| координатор | 6 постов LinkedIn (компания + личный), EN/ES, картинки | `content/social/2026-10-30-linkedin-posts.md` | review |

Следующая волна (когда освободятся потоки):
1. seo-researcher — брифы /how-it-works, /faq, /pricing (W2-03) и сравнений W3-04: PlanVIA vs Wanderlog, Wanderlog alternatives, Pilot.
2. writer — правки хаба по отчёту фактчекера.
3. social-producer — 3 сценария роликов на зимние темы (ярмарки, Новый год, лыжи с друзьями).
4. community-scout — дайджест тредов №2.
