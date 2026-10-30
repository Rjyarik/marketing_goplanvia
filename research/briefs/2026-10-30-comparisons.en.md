# Бриф: три страницы сравнений (W3-04)

Три страницы в одном брифе, потому что у них общая карточка конкурентов и общие правила:

| # | Страница | URL (предложение) | Главный запрос |
|---|---|---|---|
| A | Wanderlog alternatives | /compare/wanderlog-alternatives | **Wanderlog alternatives** (`en-04` из `data/ai-visibility-prompts.csv`, приоритет high) |
| B | PlanVIA vs Wanderlog | /compare/planvia-vs-wanderlog | **PlanVIA vs Wanderlog** (бренд-запрос, спроса пока нет) |
| C | PlanVIA vs Pilot | /compare/planvia-vs-pilot | **PlanVIA vs Pilot** (бренд-запрос, спроса пока нет) |

- Тип: сравнение
- Язык: EN. ES-вариант страницы A («alternativas a Wanderlog», `es-04`) — отдельной адаптацией позже, см. «Идеи»
- Для кого: компания из 4–8 друзей 22–33 лет и тот, кто собирает план; он уже слышал про Wanderlog (часто из TikTok) или попробовал и ищет, что подходит группе
- Сезон публикации: вторая половина ноября 2026 (W3-04, неделя 16–22 ноября). Страницы вечнозелёные, но дата «Checked» ставится в день публикации
- Задача в backlog: W3-04 и предложение про Pilot и TripProf из раздела «Идеи» · выдача и страницы конкурентов смотрел 30.10.2026
- Адреса: в документе стратегии (вкладка «Сайт», P3) для Wanderlog указан `/compare/wanderlog-alternative-for-groups`. Я предлагаю `/compare/wanderlog-alternatives`, чтобы адрес совпадал с запросом; группа остаётся в H1. Решение за координатором

## Главные находки

1. **На групповых функциях PlanVIA сегодня не выигрывает ни у Wanderlog, ни у Pilot.** Wanderlog (по описанию в App Store) даёт приглашения по email или ссылке, права «правит / смотрит» и совместное редактирование в реальном времени, плюс бюджет и деление счетов. Pilot (по собственным страницам) даёт приглашения, совместное редактирование, «сердечки» для голосования и чат поездки. В PlanVIA ничего из этого нет (`CLAUDE.md`). Раздел «Where PlanVIA is better» держится сегодня на одном-двух пунктах с непроверенным сравнением (см. «Что у PlanVIA честно лучше»). Без них страницы B и C читаются как реклама чужого продукта. Это главный аргумент выпускать B и C **после W2-01** (совместная поездка). Страницу A можно выпустить раньше: это подборка «кому что подходит».
2. **Pilot — самый сильный конкурент по нашему углу «друзья».** Бесплатный, веб, iOS и Android, ИИ-маршрут, офлайн и PDF бесплатно (по их страницам), бронирование отелей, групповые блоки номеров от 12 человек. Он целенаправленно работает на AI-ответы: у него есть [/llms.txt](https://www.pilotplans.com/llms.txt) и страница [/for-ai-assistants](https://pilotplans.com/for-ai-assistants), и он выпустил шаблонные страницы «Pilot vs X» (в выдаче я насчитал не меньше 13 продуктов). Нам нужны три ручные страницы, а не шаблон на десятки: массовая генерация попадает под правила Google о scaled content abuse (`CLAUDE.md`).
3. **Цифры Pilot друг другу противоречат.** Рейтинг 4.7 «от 120,000+ путешественников» (главная и лендинг), в том же лендинге ниже «40,000+», «50,000+ groups», в `llms.txt` «180+ verified reviews», на странице для AI «70,000+ trips» и Trustpilot 4.4. На iOS-странице (витрина США, 30.10.2026) рейтинг 5.0 по 2 оценкам. Основной продукт Pilot — веб, приложение вторично, так что 2 оценки ничего не доказывают. Вывод: **эти цифры в наши страницы не переносим.**
4. **В фактах о Wanderlog есть противоречие про офлайн**, и оно касается уже написанного хаба. В описании App Store: «All your plans are automatically stored offline». В справке Wanderlog пункт «Download trip plan for offline access» стоит в разделе **Pro features**, и в блоге основателя от 26.11.2024 офлайн только в Pro. В хабе (`content/pages/2026-10-29-group-trip-planner.en.md`, таблица «Which apps…») написано «Wanderlog stores plans offline in its app», а фактчекер поставил «pass» (строка 37 отчёта). Предлагаю поправить хаб (формулировка в «Карточке Wanderlog»).
5. **Выдача по «Wanderlog alternatives» — каталоги и страницы самих вендоров.** Каталоги (AlternativeTo, SaaSHub, PeerPush и подобные), страницы вендоров, которые ставят себя первыми (Pilot, MonkeyTravel, Stippl, TripProf), и одна редакционная подборка (ClickUp, по данным `data/outreach-targets.csv`). Ни одна из просмотренных не предлагает выбор по задаче группы и ни одна не говорит открытым текстом «мы пристрастны, вот когда лучше взять другого». Это наш угол.
6. **Что Pilot пишет о Wanderlog:** Pilot в собственном блоге (29.09.2026) пишет, что у Wanderlog «limited collaboration tools» и платные базовые функции. Это не совпадает с описанием самого Wanderlog в App Store (совместное редактирование есть, по описанию). Нам нельзя копировать такие оценки; пишем только то, что видно на официальных страницах, и называем источник.

## Общие правила для трёх страниц

1. **Раскрытие в первом абзаце:** «We make PlanVIA, so we're not neutral. Every claim about another product links to its own page and carries the date we checked it.»
2. **Ответ в первых двух предложениях** (шаблон «Сравнение» из `templates/pages.md`): кому что подходит.
3. **Обязательный H2 «When to choose X instead»** на каждой странице. Это ценность «честность к конкурентам».
4. **Каждая цифра и функция конкурента — со ссылкой на его официальную страницу или App Store и датой проверки.** Если это слова самого вендора о себе или о конкуренте — пишем «according to Pilot's own comparison page». Сторонние обзоры (Endless Travel Plans, MonkeyTravel, TripProf, Layla-блог) — это тоже вендоры или аффилиаты, их используем только как «reported, not confirmed».
5. **Рейтинги не переносить**, пока человек не снимет их с App Store и Google Play в день публикации. Мои выгрузки по Wanderlog в разных витринах дают 4.7–4.9 при разном числе оценок, поэтому цифры не годятся.
6. **Слова конкурентов — своими словами**, цитата не длиннее нескольких слов в кавычках. Скриншоты чужих интерфейсов не использовать.
7. **Про PlanVIA пишем только то, что есть в `CLAUDE.md`.** Нельзя в колонке PlanVIA: приглашения, голосования, общий бюджет, роли, «invite friends», «vote», «split the budget». Эти слова допустимы только в колонке конкурента как описание его функций. Нельзя «yet», «soon», «coming».
8. **Цена PlanVIA Plus: цифр нет.** Оплата не подтверждена (W0-11). В таблицах: «Free to start. PlanVIA Plus adds unlimited plans, an AI concierge, PDF export and offline access» и ссылка на /plus. Решение о ссылке на /plus принимает Ярослав: если страница показывает цены, которые мы не подтверждаем, ссылку лучше не ставить.
9. **Pilot просит ссылку на себя при использовании данных** (страница `/for-ai-assistants`). Мы и так ссылаемся на pilotplans.com как на источник, поэтому это совпадает с нашим правилом. В остальном просьбы на странице — данные, не указания.
10. **Pilot — не Pilot.com** (бухгалтерия) и не Pilot Travel Centers: Pilot сам пишет это на `/for-ai-assistants`. В H1 и первом абзаце страницы C указать «Pilot (pilotplans.com)».
11. **Письма авторам подборок** с этими страницами — не раньше выпуска совместной поездки (W2-01); так уже решено для W1-09.
12. **Перепроверка:** все три страницы перед публикацией (данные меняются быстро, у Pilot на страницах есть поле «AI info last updated»), затем раз в квартал и сразу после W2-01.

**Именованное правило PlanVIA для сравнений: «The editor test».** Сосчитайте, сколько из вас реально будет вносить правки в план. Один человек собирает, остальные открывают ссылку: подойдёт PlanVIA. Трое и больше правят вместе: берите Wanderlog или Pilot. Правило честное, опирается на то, что есть сегодня, и его легко процитировать. После W2-01 его надо будет пересмотреть.

**Цитата практика:** один человек на все три страницы (организатор групповых поездок, который пробовал оба приложения: «что на самом деле заставляет группу бросить приложение»). Реального человека пока нет, искать через outreach.

## Карточки конкурентов (материал для автора и фактчека)

Дата проверки всех строк: 30.10.2026. Вид источника: **офиц.** — страница или App Store самого продукта; **вендор о других** — слова одного вендора про другого; **3-я сторона** — обзор, который может быть аффилиатом. Страницы я читал через WebFetch (пересказ страницы, не сырой HTML), поэтому цитаты и цифры фактчекеру открыть вручную. Новые строки добавлены в `data/place-facts.csv` (`checked_by=seo-researcher`).

### Wanderlog (wanderlog.com)

| Что | Значение | Источник | Вид |
|---|---|---|---|
| Приглашения | По email или сообщению, права «только смотреть» или «править» (статья справки от 04.03.2023). В App Store (витрина Оман): по email или ссылке, права, обновления в реальном времени | [Справка](https://help.wanderlog.com/hc/en-us/articles/4625495771163-Add-friends-to-plan-together); [App Store](https://apps.apple.com/om/app/id1476732439) | офиц. |
| Совместное редактирование | «Invite friends and collaborate in real-time just (like Google Docs)» | [App Store, витрина США](https://apps.apple.com/us/app/wanderlog/id1476732439) | офиц. |
| Нужен ли друзьям аккаунт | В справке не сказано | — | не подтверждено |
| Голосование, чат | В справке и описании App Store не нашёл. Pilot, TripProf и MonkeyTravel пишут, что их нет | см. ниже | не подтверждено самим Wanderlog. В тексте: «we didn't find a voting feature in Wanderlog's help center» |
| Расходы | «Free travel expense and budgeting app», деление с друзьями, «who owes who», валюта траты и домашняя валюта, правка расходов офлайн в мобильном приложении | [wanderlog.com](https://wanderlog.com/travel-budget-expense-splitting-app) (без даты, © 2025) | офиц. |
| AI | Подсказки мест, оптимизация маршрута, автозаполнение дней; места ранжируются по отзывам Tripadvisor и Google. Ассистент у Pro-пользователей после 5 бесплатных сообщений (блог, 26.11.2024). Сегодняшний лимит не проверен | [wanderlog.com/trip-planner-ai](https://wanderlog.com/trip-planner-ai); [блог основателя, 26.11.2024](https://wanderlog.com/blog/2024/11/26/wanderlog-vs-tripit/) | офиц. |
| Цена Pro | $39.99 в год (блог основателя 26.11.2024 и 14.10.2024). В 2026 году те же $39.99 называют Endless Travel Plans (июль), MonkeyTravel (сентябрь), TripProf и Pilot. В App Store несколько цен по витринам. **[проверить вручную]** в приложении | [блог, 14.10.2024](https://wanderlog.com/blog/2024/10/14/is-there-a-free-trip-planner/) | офиц. (2024) + 3-я сторона (2026) |
| Что в Pro | Скачивание плана и гайдов офлайн, оптимизация маршрута, сканирование Gmail (справка, раздел «Pro features»). Экспорт в Google Maps (App Store) | [Справка, Pro features](https://help.wanderlog.com/hc/en-us/sections/13302911983643--Pro-features) | офиц. |
| Офлайн | **Противоречие.** App Store: «All your plans are automatically stored offline». Справка и блог 26.11.2024: офлайн-скачивание в Pro; в блоге 14.10.2024 «basic itinerary access offline is included in the free version», а офлайн-карты в Pro | см. выше | офиц., но источники расходятся. В тексте: «offline downloads are listed as a Pro feature in Wanderlog's help center; check the app before you rely on it» |
| Платформы | Веб, iOS, Android | [wanderlog.com/download-android-app](https://wanderlog.com/download-android-app) (редирект в Google Play); App Store | офиц. |
| Пользователи | «Over 1 million people have already tried Wanderlog» | [wanderlog.com](https://wanderlog.com/) | офиц. (заявление компании, без даты) |
| Рейтинги | Не переносим (см. правило 5) | — | — |

**Не использовать:** [wanderlog.com/blog/faq](https://wanderlog.com/blog/faq/) — страница устарела (там написано, что учёта расходов нет), противоречит текущим страницам.

### Pilot (pilotplans.com, HappyHour Services Inc., Ванкувер)

| Что | Значение | Источник | Вид |
|---|---|---|---|
| Что это | «Free, AI-powered collaborative trip booking and planning app»; веб-приложение (app.pilotplans.com), iOS, Android | [llms.txt](https://www.pilotplans.com/llms.txt); [главная](https://pilotplans.com/) | офиц. |
| Цена | Бесплатно; опциональный платный уровень «pay what you want»; зарабатывает на бронированиях отелей и платных услугах | [/group-trip-planner](https://www.pilotplans.com/group-trip-planner) (в странице «AI info last updated: May 2026») | офиц. |
| Групповые функции (лендинг) | Несколько человек правят один план, обновления синхронизируются; вкладка «Files» с подтверждениями; идеи и «maybes»-список. **Про голосование и чат на лендинге не нашёл** | та же страница | офиц. |
| Групповые функции (их сравнение с Wanderlog, страница обновлена 29.09.2026) | Приглашения: да. Совместное редактирование: да. Права «правит / смотрит»: да. «Heart items for voting»: да. Групповой чат: да. Деление расходов между людьми: **нет**; бюджет и расчёт на человека: «Partial» | [Pilot vs. Wanderlog, feature comparison](https://www.pilotplans.com/compare/wanderlog-alternative-feature-comparison) | вендор о других и о себе. **Проверить в приложении** (нужна регистрация) |
| Офлайн и PDF | Бесплатно (заявление Pilot) | страницы выше | офиц. (заявление) |
| Бронирование | Отели в приложении (на странице для AI названо 3.2M+ отелей-партнёров); перелёты через поиск Skyscanner (бронь вне приложения); групповые блоки номеров для групп от 12 человек | [/for-ai-assistants](https://pilotplans.com/for-ai-assistants) (заголовок «July 2026», подвал «May 2026») | офиц. |
| iOS | Версия 1.8.0, «free travel app for friends to discover activities and plan & share trips», только iPhone, iOS 16.4+, язык интерфейса — английский, рейтинг 5.0 по 2 оценкам (витрина США, 30.10.2026) | [App Store](https://apps.apple.com/us/app/id6446177269) | офиц. |
| Языки | Английский (по App Store). Веб-версию на других языках не проверял | — | не подтверждено |
| Заявления о размере | 4.7 от «120,000+» и «40,000+»; «50,000+ groups»; «183 countries»; «180+ verified reviews»; «70,000+ trips» | страницы выше | офиц. (заявления противоречат друг другу, **не переносим**) |
| Как оценивает Wanderlog | «Limited collaboration», платные базовые функции, «clunky» (блог Pilot, 29.09.2026) | [блог Pilot](https://www.pilotplans.com/blog/best-trip-planner-apps) | вендор о других. Не повторяем |

### Другие альтернативы для страницы A

| Продукт | Что нашёл | Источник | Вид |
|---|---|---|---|
| Mindtrip | Бесплатный. «Planning with friends? Share ideas, invite others to collaborate…»; групповые чаты и общие подборки/маршруты; бронь перелётов, жилья, ресторанов, активностей; веб и iOS (Android в FAQ не упомянут); разговорный слой на OpenAI | [FAQ](https://resources.mindtrip.ai/travelers/help/traveler-faqs.md); [App Store](https://apps.apple.com/app/id6503107567) | офиц. |
| Layla | Планирование бесплатное, поездки под ключ бронируют эксперты, рекомендуемый минимум €100 на человека за ночь (строки 23–24, 39 `place-facts.csv`). Премиум-подписка $49 в год (PriceLock) по их же блогу от 02.06.2026. **Вывод: нельзя писать «Layla has no subscription», у неё две отдельные схемы** | [layla.ai](https://layla.ai/); [блог, 02.06.2026](https://layla.ai/blog/destinations/ai-trip-planners-tier-list) | офиц. |
| Stippl | Совместное планирование (приглашение со-планировщика), в бюджете деление счетов в группе, AI-планировщик в Pro, полный офлайн; бесплатно с покупками, цены Pro в UK-витрине £3.99, £24.99, £29.99 (периоды не указаны) | [App Store, UK](https://apps.apple.com/gb/app/id6443617088?l=en-gb) | офиц. |
| TripProf | Бесплатно соло-планирование; «1 credit = 1 trip» открывает групповую работу, автоматизацию и офлайн; пакеты от €3.99, месяц €7.99 за 3 кредита, год €54.99 за 36; сами пишут «no built-in group voting»; интерфейс EN и DE по их тексту | [блог TripProf, 17.03.2026, обновл. 19.09.2026](https://tripprof.com/en/blog/best-group-travel-planning-apps/) | офиц. (блог вендора). Цены на странице тарифов **[проверить вручную]** |
| TripIt | Блог TripIt (21.01.2026) советует TripIt для общего маршрута из пересланных писем, а для связи, расходов и упаковки — WhatsApp, Splitwise, Venmo, PackPoint. Групповое редактирование не заявлено. Цену Pro взять с tripit.com **[проверить вручную]** | [блог TripIt](https://www.tripit.com/web/blog/travel-tips/best-group-travel-planning-app) | офиц. |

## Страница A: Wanderlog alternatives

- URL: /compare/wanderlog-alternatives
- Главный запрос: **Wanderlog alternatives**. Побочные: «apps like Wanderlog», «Wanderlog alternative for groups», «free alternative to Wanderlog» — объём не проверен
- Что хочет человек: понять, что взять вместо Wanderlog или кроме него; часто — AI, голосование, чат, бесплатный офлайн

### Запросы

| # | Запрос | Интент | Где | Объём |
|---|---|---|---|---|
| 1 | Wanderlog alternatives | сравнение | Google, ChatGPT | объём не проверен |
| 2 | apps like Wanderlog | сравнение | Google | объём не проверен |
| 3 | Wanderlog alternative free | цена | Google | объём не проверен |
| 4 | Wanderlog alternative for groups | группа | Google, ChatGPT | объём не проверен |
| 5 | Wanderlog vs Layla (`en-12`) | сравнение | ChatGPT | объём не проверен |
| 6 | is Wanderlog free / is Wanderlog worth it | цена | Google | объём не проверен |
| 7 | Wanderlog with voting | функция | Google | объём не проверен |

### Вопросы для H2

1. **What are the best Wanderlog alternatives for a group trip?** Ответ — по задаче, одним предложением на продукт:
   - все правят и голосуют в бесплатном приложении: Pilot (по его страницам);
   - AI-чат строит и бронирует: Layla (планирование бесплатное, поездки под ключ бронируют эксперты) или Mindtrip (бесплатный, групповые чаты);
   - общий маршрут из писем с бронями: TripIt;
   - аккуратный визуальный планировщик с AI в Pro: Stippl;
   - группе нужны кредиты на поездку: TripProf;
   - один человек собирает план, остальные смотрят; готовые планы и бронь поездов, авто, eSIM: PlanVIA (мы).
2. **Why do people look for a Wanderlog alternative?** Причины с источниками: бесплатный AI ограничен (по Wanderlog 2024 — 5 сообщений; MonkeyTravel называет около 5 на поездку по обзору февраля 2026), офлайн в Pro, голосования и чата нет (по Pilot, TripProf, MonkeyTravel), «gets slower the more you add» (отзыв на r/travel, август 2024, в пересказе Endless Travel Plans, июль 2026). Тон нейтральный. Рейтинг Trustpilot (1.8 по 48 отзывам, Endless Travel Plans, июль 2026) — только если автор откроет Trustpilot сам и поставит дату.
3. **Which Wanderlog alternative has group voting or chat?** Pilot (по собственной странице сравнения: сердечки и чат), Mindtrip (групповые чаты), остальные — нет по их же описаниям; PlanVIA — нет. Перед публикацией человек с аккаунтами должен открыть Pilot и Mindtrip и подтвердить.
4. **Which Wanderlog alternatives are free?** Таблица цен (см. ниже).
5. **When should you stay with Wanderlog?** Обязательный раздел: когда трое и больше правят план одновременно и хотят бесплатный совместный режим; когда нужны встроенные расходы с делением; планирование road trip с оптимизацией маршрута (Pro); письма с бронями в Gmail (Pro); у продукта миллион пользователей и годы работы. Даже конкурент Layla в своём блоге (02.06.2026) называет Wanderlog «best collaborative trip organizer, especially for road trips».
6. **How do you choose in two minutes?** The editor test + четыре вопроса: сколько из нас правят план; нужен ли чат и голосование внутри; нужен ли встроенный учёт расходов; нужен ли бесплатный офлайн.

**FAQ (H3):** Is Wanderlog free? · What is the best free alternative to Wanderlog? · Does Wanderlog have AI? · Is there a Wanderlog alternative with voting? (источники — в «Карточке»).

### Что в таблице с цифрами

**Таблица 1. «Wanderlog alternatives at a glance».** Строки: Pilot · Mindtrip · Layla · Stippl · TripProf · TripIt · PlanVIA (последней, с пометкой «ours»). Столбцы: Best for · Group tools (invite / edit together / vote / chat) · AI itinerary · Free or paid (цена с валютой и периодом) · Platforms · Source · Checked.
**Таблица 2. «What it costs»** — только из «Карточек» выше. Wanderlog Pro $39.99 в год (оговорка про 2024 и витрины), Pilot free, Layla $49 в год премиум, Stippl £3.99/£24.99/£29.99 (периоды не указаны), TripProf €3.99/€7.99/€54.99, PlanVIA Plus — без цены.
В каждой ячейке «Source» — ссылка и дата; пустые ячейки, где данных нет, и подпись «not checked», а не догадка.

### Что в выдаче и AI-ответах сейчас

Выдачу смотрел через WebSearch 30.10.2026 (индекс США, не Google напрямую). Ответы ChatGPT и Perplexity не снимал (W1-04 заблокирован).

- **Каталоги и агрегаторы:** AlternativeTo (по Wanderlog много страниц по 11 альтернатив), SaaSHub, PeerPush, Toolmage, Sugggest, seektool и страницы на `*.pages.dev`. Описания короткие, без цен и без группового угла.
- **Вендоры, которые ставят себя первыми:** [MonkeyTravel](https://monkeytravel.app/blog/wanderlog-alternative-2026) (27.07.2026, обновл. 28.10.2026) рекомендует только себя; [Pilot](https://www.pilotplans.com/compare/wanderlog-alternative) (обновл. 11.06.2026) и вторая его страница сравнения; Stippl и TripProf.
- **Редакционные:** ClickUp «Top 8 Wanderlog Alternatives…» (по `data/outreach-targets.csv`, статью сам не открывал: URL не в allowlist) — единственная независимая подборка, есть испанская версия.
- **Wanderlog о себе:** свои блоги 2024 года («Is There a Free Trip Planner?», «Wanderlog vs TripIt»).

**Чего не хватает группе.** Нет страницы, которая выбирает по задаче группы и честно говорит, где что слабо. Нет сравнения «сколько человек правят». Почти нигде не видно даты проверки цены.

### Метаданные (черновик)

- Title (58 символов): `Wanderlog Alternatives for Group Trips, Compared | PlanVIA`
- Description (145 символов): `Wanderlog alternatives for a trip with friends: who has voting, group chat, free offline and AI itineraries. Honest comparison, checked Nov 2026.`
- Заголовок превью: `Wanderlog alternatives for group trips`
- Подзаголовок превью: `Who has voting, chat and free offline`

## Страница B: PlanVIA vs Wanderlog

- URL: /compare/planvia-vs-wanderlog
- Главный запрос: **PlanVIA vs Wanderlog**; заодно «Wanderlog vs», «how is PlanVIA different from Wanderlog» (вопрос FAQ главной в плане). Запросов у бренда пока нет: страница нужна для AI-ответов, как цель ссылки на странице A и в FAQ, и для писем авторам подборок после W2-01

### Вопросы для H2

1. **Which is better for a group trip, PlanVIA or Wanderlog?** Короткий ответ по правилу «The editor test»: один человек собирает — PlanVIA; трое и больше правят — Wanderlog.
2. **How do PlanVIA and Wanderlog compare side by side?** Таблица (ниже).
3. **Can several friends edit the plan at the same time?** Wanderlog — да, в реальном времени, по приглашению (по App Store и справке). PlanVIA — нет: план собирает один человек, остальные открывают ссылку (**подтвердить**, `plan/questions.md` п. 2).
4. **How do their AI itineraries differ?** Wanderlog: ассистент в Pro после 5 бесплатных сообщений (блог 2024), места ранжируются по отзывам Tripadvisor и Google. PlanVIA: маршрут по дням с картой и реальными местами для 100+ направлений; AI-консьерж в Plus. Лимит бесплатного AI в PlanVIA неизвестен: не сравнивать «кто щедрее».
5. **What do they cost?** Wanderlog: бесплатно, Pro около $39.99 в год (дата, оговорка). PlanVIA: free to start, Plus — состав без цен.
6. **When should you choose Wanderlog instead?** (обязательный) см. страницу A, раздел 5.
7. **When does PlanVIA fit better?** См. «Что у PlanVIA честно лучше».

### Что в таблице с цифрами

Шаблон «Сравнение» из `templates/pages.md` (Для чего лучше · Цена · Работа с группой · AI-маршрут), расширенный.

| | PlanVIA | Wanderlog |
|---|---|---|
| Best for | Один человек собирает план по дням (с нуля или из готового) и делится им | Несколько человек вместе наполняют план, плюс расходы |
| Price | Free to start. Plus: безлимит планов, AI-консьерж, PDF, офлайн. Цен нет (W0-11) | Free. Pro около $39.99 в год (блог основателя 26.11.2024 и обзоры 2026), **[проверить вручную]** |
| Group work | Share the plan. Приглашений, ролей, голосования нет | Приглашение по email или ссылке, права, правки в реальном времени |
| Voting and chat | Нет | В справке не нашёл (по Pilot, TripProf: нет) |
| Expenses | Нет (используйте Splitwise или Tricount) | Бюджет, траты, деление счетов |
| AI itinerary | День за днём, карта, реальные места, 100+ направлений | Ассистент (5 бесплатных сообщений в 2024), оптимизация маршрута |
| Offline | В Plus | Скачивание офлайн указано в Pro (справка); App Store пишет, что планы хранятся офлайн: противоречие |
| Booking | Партнёры: перелёты, поезда, авто, eSIM, отели | Нашёл только заявленные в обзорах предложения на перелёты и авто в Pro **[проверить вручную]** |
| Platforms | **[вопрос Ярославу: веб, приложение?]** | Веб, iOS, Android |
| Interface languages | EN, ES, RU, DE | **[не проверено]** |

Для каждой строки автор ставит источник и «Checked: Nov 2026».

### Метаданные (черновик)

- Title (55 символов): `PlanVIA vs Wanderlog: Which Is Better for a Group Trip?`
- Description (149 символов): `PlanVIA vs Wanderlog side by side: group editing, AI itinerary, offline, booking and price. Where Wanderlog is the better pick, and where PlanVIA is.`
- Заголовок превью: `PlanVIA vs Wanderlog`
- Подзаголовок превью: `Which fits your group, with sources`

## Страница C: PlanVIA vs Pilot

- URL: /compare/planvia-vs-pilot
- Главный запрос: **PlanVIA vs Pilot**; побочные «Pilot trip planner», «Pilot group trip planner vs», «Pilot vs Wanderlog»
- Особенность: самый сильный конкурент по нашему углу и самый честный текст. Если выпускать до W2-01, страница прямо скажет: **по групповым инструментам сегодня сильнее Pilot** (по его же странице сравнения). Для ценности «честность к конкурентам» это верно, но для позиционирования рискованно: решение Ярослава.

### Вопросы для H2

1. **Which is better for planning a trip with friends, PlanVIA or Pilot?** Ответ: если вы хотите, чтобы вся компания правила, голосовала и переписывалась внутри приложения, сегодня выберите Pilot (по его страницам). Если один человек собирает план из готового маршрута и делится ссылкой, PlanVIA подходит не хуже.
2. **How do PlanVIA and Pilot compare side by side?** Таблица ниже.
3. **Does Pilot have voting and group chat?** По собственной странице сравнения (обновлена 29.09.2026) — да (сердечки и чат), на лендинге и в `llms.txt` об этом не сказано. **Человек с аккаунтом проверяет в приложении.** В PlanVIA нет ни того, ни другого.
4. **What does each one cost, and how does it make money?** Pilot: бесплатно, опциональный платный уровень по принципу «pay what you want», доход с бронирований отелей и платных услуг. PlanVIA: free to start, Plus, цены не указываем.
5. **Which one books more of the trip?** Pilot: отели в приложении и поиск рейсов через Skyscanner (бронь вне приложения), групповые блоки от 12 человек. PlanVIA: перелёты, поезда, аренда авто, eSIM, отели у партнёров (с раскрытием партнёрских ссылок). **Проверить у Pilot, нет ли поездов, авто и eSIM.**
6. **Which one works offline and exports a PDF?** Pilot: бесплатно (заявление). PlanVIA: в Plus.
7. **When should you choose Pilot instead?** (обязательный) Список из пяти пунктов: правят втроём и больше; нужно голосование и чат; нужен бесплатный офлайн и PDF; нужен блок номеров для группы от 12 человек; нужно мобильное приложение для Android и iOS (если у PlanVIA его нет, **вопрос Ярославу**).
8. **When does PlanVIA fit better?** См. «Что у PlanVIA честно лучше».

### Что в таблице с цифрами

| | PlanVIA | Pilot (pilotplans.com) |
|---|---|---|
| Best for | Один человек собирает план, группа смотрит ссылку | Группа, которая правит и обсуждает внутри приложения |
| Price | Free to start; Plus без цен | Free; опциональный платный уровень «pay what you want» |
| Group work | Share the plan | Приглашения, правка вместе, права (по их сравнению, 29.09.2026) |
| Voting and chat | Нет | «Hearts» и чат поездки (по их сравнению; проверить в приложении) |
| Expenses | Нет | «Partial»: бюджет и расчёт на человека; деления расходов между людьми нет (их же слова) |
| AI itinerary | День за днём, карта, реальные места, 100+ направлений | AI-маршрут с фильтрами (60+ по `llms.txt`, 50+ по лендингу) |
| Offline and PDF | Plus | Бесплатно (заявление Pilot) |
| Booking | Партнёры: перелёты, поезда, авто, eSIM, отели | Отели (3.2M+ по их странице), рейсы через Skyscanner, блоки номеров от 12 |
| Platforms | **[вопрос]** | Веб, iOS, Android |
| Interface languages | EN, ES, RU, DE | Английский (App Store) |

Цифры размера аудитории Pilot (120,000+, 50,000+ и др.) в таблицу не ставить: они противоречат друг другу (находка 3).

### Метаданные (черновик)

- Title (52 символа): `PlanVIA vs Pilot: Trip Planners for Friends Compared`
- Description (143 символа): `PlanVIA vs Pilot (pilotplans.com) for a trip with friends: group tools, AI itinerary, booking, offline and cost. When Pilot is the better pick.`
- Заголовок превью: `PlanVIA vs Pilot`
- Подзаголовок превью: `Two trip planners for friends, compared`

## Что у PlanVIA честно лучше (одно место для автора всех трёх страниц)

Из `CLAUDE.md`. Каждый пункт помечен, насколько он подтверждён сравнением с конкурентом.

| Пункт | Статус сравнения |
|---|---|
| Бронирование поездов, аренды авто и eSIM рядом с перелётами и отелями | У Pilot нашёл отели и поиск рейсов, у Wanderlog предложения Pro по перелётам и авто (по обзорам). Поездов и eSIM у них не видел. **Перед публикацией открыть страницы бронирования обоих** |
| Интерфейс на испанском, немецком, русском | Pilot: английский (App Store). Wanderlog: не проверил. **Проверить** |
| Каталог готовых планов: открыть, скопировать, поправить | Есть ли у Pilot и Wanderlog копируемые публичные маршруты, не проверил. **Проверить**. Зависит и от W2-02 (копирование без регистрации) |
| Кошелёк билетов (PDF, картинки) | У Pilot вкладка «Files», у Wanderlog импорт броней из Gmail (Pro). Не отличие |
| Проверенные страницы городов с ценой на человека и датой | Это содержание сайта, а не функция. Для сравнений можно ссылаться, как на «what's in our catalogue» |

**Вывод для координатора:** без выпуска совместной поездки (W2-01) раздел «Where PlanVIA is better» состоит из одной-двух строк, которые ещё надо подтвердить. Предлагаю: A выпускать в ноябре, B и C — после W2-01 или, если Ярослав решит иначе, в честной версии «who we recommend today».

## Факты, которые надо проверить

| Факт | Где проверять |
|---|---|
| Что есть в PlanVIA: 100+ направлений, каталог, 5 категорий бронирования, Plus, кошелёк, 4 языка | `CLAUDE.md`, «Продукт: что есть сейчас» |
| Как работает ссылка на план; можно ли править ссылку; нужен ли вход | `plan/questions.md` п. 2; W2-02 |
| Платформы PlanVIA: только веб или есть приложение | `plan/questions.md` п. 5 |
| Лимит бесплатных планов и бесплатного AI | `plan/questions.md` п. 1 |
| Цены Plus, оплаты | `plan/questions.md` п. 3; W0-11 |
| Раскрытие партнёрских ссылок | `plan/questions.md` п. 12 |
| Wanderlog: Pro-цена сегодня, лимит бесплатного AI сегодня, офлайн в бесплатной и Pro-версии, голосования и чат (в приложении) | приложение и страница оплаты Wanderlog, человек с аккаунтом и телефоном |
| Wanderlog: языки интерфейса, рейтинги App Store и Google Play | App Store и Google Play в день публикации |
| Pilot: голосование, чат, приглашения, расходы, языки веб-версии, Android | приложение Pilot, аккаунт |
| Pilot: поезда, авто, eSIM в бронировании | app.pilotplans.com |
| Mindtrip: групповые чаты, цена, Android | mindtrip.ai, App Store и Google Play |
| Layla: условия бесплатной части и премиума; может ли друг править поездку (документ стратегии ссылается на Aizzie, «перепроверить в день публикации») | layla.ai |
| Stippl: периоды и цены Pro, групповые функции | stippl.io, App Store |
| TripProf: цены тарифов, число языков | tripprof.com (страница тарифов) |
| TripIt: цена Pro, групповые функции | tripit.com |
| ClickUp: что в подборке и дата (я статью не открывал) | clickup.com/blog/wanderlog-alternatives |
| Реальный автор, цитата практика | `plan/questions.md` п. 11; outreach |

## Маршрут или шаблон PlanVIA

<план из каталога, открывающийся без регистрации: уточнить у координатора>

Финал страниц A, B, C — «Copy this itinerary» (например, Lisbon, 3 days) и «Create a trip». Пока W2-02 не сделан, автор не обещает «no sign-up». На странице A ссылки на B и C; на B и C ссылка на хаб /group-trip-planner и на /how-it-works.

## Риски и вопросы координатору

1. **Порядок выпуска.** Рекомендую A в ноябре, B и C — после W2-01. Решение за Ярославом.
2. **Хаб содержит устаревшую строку про офлайн Wanderlog.** Исправить на «Wanderlog lists offline downloads as a Pro feature in its help center» (и обновить строку 21/38 в `place-facts.csv` пометкой; я добавил отдельную строку, старые не менял).
3. **Предыдущий бриф хаба** (2026-10-29) пишет, что у Pilot «голосования и деления расходов на странице нет». На лендинге это верно, но на странице сравнения Pilot сам заявляет «heart items for voting» и чат. Поправить формулировку.
4. **Документ стратегии** в строке сравнений говорит «PlanVia» в title (нужно PlanVIA) и ссылается на Aizzie для Layla (перепроверить).
5. **Пилотные оценки Pilot о Wanderlog** (блог 29.09.2026) агрессивны. Не повторяем и не отвечаем в тоне.
6. **Мой доступ к конкурентам ограничен:** приложения и платные страницы из среды не открываются, голосование, чат и актуальные цены можно проверить только руками. Список в «Фактах».

## Вопросы Ярославу

1. Порядок выпуска: сначала A, а B и C после совместной поездки (W2-01), или все три в ноябре в честной версии «who we recommend today»?
2. Есть ли у PlanVIA мобильное приложение или только веб (`plan/questions.md` п. 5)? Это строка «Platforms» в двух таблицах.
3. Можно ли в сравнениях ссылаться на /plus без цифр, пока оплата Plus не подтверждена?
4. Согласны ли на правило «The editor test» как именованное правило сравнений?
5. Кто может с аккаунтом за 15 минут проверить в приложениях Pilot и Wanderlog голосование, чат, лимит бесплатного AI и актуальную цену Pro?
