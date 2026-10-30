# Backlog: план на 90 дней

Источник — вкладка «План на 90 дней» в документе стратегии. Координатор держит статусы здесь и в документе одинаковыми.

Статусы: `todo` · `doing` · `review` (ждёт Ярослава) · `done` · `blocked`.
Исполнитель: роль из `.claude/agents/` или «Ярослав».

## Неделя 0 (29 октября – 1 ноября): запуск системы

| ID | Задача | Исполнитель | Статус | Заметки |
|---|---|---|---|---|
| W0-01 | goplanvia.com — основной домен в Lovable, редирект с yourplanvia.com | Ярослав | done | Редирект Lovable работает |
| W0-02 | Подтвердить goplanvia.com в Search Console, Bing, Meta | Ярослав | todo | |
| W0-03 | Репозиторий marketing_goplanvia | Ярослав | done | |
| W0-04 | Claude GitHub App на marketing_goplanvia | Ярослав | done | Push работает с 28.10 |
| W0-05 | Проект в Claude Code, инструкции проекта | Ярослав | review | Со слов Ярослава создан; проверить инструкции из раздела 5 «Команды агентов» |
| W0-06 | Коннекторы: n8n (MCP), BabyLoveGrowth | Ярослав | todo | |
| W0-07 | Ники @planvia / @goplanvia в TikTok, Instagram, YouTube, Reddit, X | Ярослав | todo | |
| W0-08 | Заполнить репозиторий: CLAUDE.md, роли, шаблоны, таблицы | координатор | done | |
| W0-09 | Домен в коде, бренд-линия, превью страниц | developer → Lovable | review | Сделано в превью Lovable; нужно опубликовать и проверить ссылку /plans в Telegram |
| W0-10 | Исправить вход через Google и Apple в Supabase | Ярослав | todo | По отчёту Lovable: Site URL = localhost, нет секрета Google, ключ Apple не принят |
| W0-11 | Проверить, принимает ли сайт реальные оплаты Plus | Ярослав + developer | todo | В коде публичный ключ Stripe тестовый (pk_test), в roadmap Lovable «Plus payments» не завершено. Без живых оплат акция к Чёрной пятнице (W4-02) бессмысленна |

## Неделя 1 (2–8 ноября): фундамент и замер

| ID | Задача | Исполнитель | Статус | Заметки |
|---|---|---|---|---|
| W1-01 | Проверить, видят ли боты превью страниц; если нет — пререндеринг | developer | todo | Зависит от W0-09 |
| W1-02 | События GA4: plan_shared, invite_sent, invite_accepted; канал «AI-ассистенты»; UTM | developer | todo | sign_up и trip_created уже есть (релиз 1.9) |
| W1-03 | Спецификация совместной поездки: ссылка-приглашение, вход друга, голосование, комментарии | координатор + Ярослав | doing | Черновик — `plan/specs/group-trip-mvp.md` |
| W1-04 | Базовый AI-замер, 30 промптов EN/ES | analyst | blocked | Подключённый n8n — не тот (нет OpenRouter); ждём коннектор к n8n на VPS |
| W1-05 | Настроить BabyLoveGrowth по разделу 9 «Стратегии» | Ярослав | todo | |
| W1-06 | Профили в каталогах AI-инструментов: There's An AI For That, Futurepedia, AlternativeTo, Product Hunt | outreach | review | Тексты: content/outreach/2026-10-29-directory-profiles.md. Бесплатно — PH и AlternativeTo; TAAFT от $49, Futurepedia $197–497, Toolify $99 — решение Ярослава |
| W1-07 | 50 микрокреаторов ES/EN | outreach | doing | 25 из 50 в data/creators.csv, проверен по-настоящему 1: Instagram/TikTok/YouTube из среды агентов не открываются. Топ-5 к первым письмам — content/outreach/2026-10-30-creators-report.md |
| W1-08 | 2 аккаунта Reddit отвечают без ссылок | Ярослав | todo | Первый дайджест черновиков — 29.10 |
| W1-09 | Цели аутрича: подборки «AI trip planner», «Wanderlog alternatives» | outreach | review | 25 целей в data/outreach-targets.csv; групповым подборкам писать после запуска совместных поездок |
| W1-10 | Первые записи /travel-alerts | alerts-monitor → fact-checker | review | 9 записей с правками фактчекера в content/alerts (+ общий день забастовок во Франции 5.11). Публиковать некуда, пока нет страницы /travel-alerts (W2-03) |

## Неделя 2 (9–15 ноября): продуктовая петля и ключевые страницы

| ID | Задача | Исполнитель | Статус | Заметки |
|---|---|---|---|---|
| W2-01 | Совместная поездка работает на сайте — рубеж | developer | todo | Без неё креаторы не говорят «с друзьями» |
| W2-02 | Открытая ссылка на план с превью и «Скопировать поездку» без регистрации | developer | todo | Превью каталожных планов уже есть (W0-09) |
| W2-03 | Страницы P1 EN+ES: /group-trip-planner (хаб), /how-it-works, /faq, /about, /pricing, /travel-alerts | seo-researcher → writer → fact-checker | doing | Бриф хаба готов. Адрес хаба — /group-trip-planner: /plan/... занят маршрутом /plan/:tripId |
| W2-04 | Цены и часы мест для 20 городов | writer + fact-checker | todo | |
| W2-05 | 10 страниц городов и 10 маршрутов «3 days in X with friends» (под весну–лето 2027) | writer | doing | Брифы: Лиссабон (EN), Semana Santa en Oporto (ES) |
| W2-06 | Письма 20 креаторам | outreach | todo | Каждое — после «да» Ярослава |

## Неделя 3 (16–22 ноября): контент-конвейер

| ID | Задача | Исполнитель | Статус |
|---|---|---|---|
| W3-01 | Ежедневный мониторинг ограничений, /travel-alerts раз в неделю | alerts-monitor | todo |
| W3-02 | 1–2 ролика в день, 3 карусели в неделю, черновики в Postiz | social-producer | doing — 6 постов LinkedIn EN/ES на одобрении (content/social/2026-10-30-linkedin-posts.md) |
| W3-03 | Ярмарки, Новый год, лыжи с друзьями — в ролики и Reddit; страницы сайта — под весну и лето 2027 | social-producer, writer | todo |
| W3-04 | Сравнения: Best apps for planning a group trip, PlanVIA vs Wanderlog, Wanderlog alternatives | seo-researcher, writer | todo |
| W3-05 | Письма 20–30 авторам подборок | outreach | todo |
| W3-06 | Письма после регистрации: пригласи друзей, отсчёт до поездки, ограничения | developer | todo |
| W3-07 | Первые ответы на Reddit, без ссылок | Ярослав + community-scout | todo |

## Неделя 4 (23–29 ноября): первая волна

| ID | Задача | Исполнитель | Статус |
|---|---|---|---|
| W4-01 | Первые 5–10 роликов креаторов | outreach | todo |
| W4-02 | Акция на Plus к Чёрной пятнице, 27 ноября | social-producer + Ярослав | todo |
| W4-03 | Посты о запуске: Indie Hackers, r/SideProject, заявка в BetaList | outreach | todo |
| W4-04 | Отчёт за месяц и второй AI-замер | analyst | todo |
| W4-05 | Рубеж 30 ноября: что удваиваем, что режем | координатор + Ярослав | todo |

## Декабрь и январь

Задачи — во вкладке «План на 90 дней», разделы «Декабрь» и «Январь». Координатор переносит их сюда в конце ноября.

## Идеи

Сюда агенты дописывают предложения с пометкой `[предложено]`. Координатор раз в неделю решает, что взять в работу.

- `[предложено]` alerts-monitor: запись /travel-alerts «Lisbon historic lifts in 2027». По RFM от 02.09.2026 Santa Justa, Glória, Bica и Lavra закрыты, Graça работает с 30.04.2026; подтвердить на carris.pt. Конкуренты (Layla, Earth Trekkers) всё ещё ставят их в маршруты. Источник — бриф `research/briefs/2026-10-29-lisbon-3-days-friends.en.md` (seo-researcher, 28.10.2026)
- `[предложено]` seo-researcher → writer: добавить Pilot и TripProf в сравнения W3-04. У Pilot сильный лендинг /group-trip-planner (50,000+ groups, FAQ из 11 вопросов) и страницы /compare/…; TripProf делает «3 Days in <City> With Friends» на 8+ языках и подборки «best group travel planning apps 2026». Возможна страница «PlanVIA vs Pilot» (seo-researcher, 28.10.2026)
