# Профили PlanVIA для каталогов AI-инструментов

- Задача: W1-06 (`plan/backlog.md`)
- Роль: outreach
- Подготовлено: 28.10.2026, проверка каталогов — 28.10.2026
- Статус: черновик, ждёт Ярослава. Ничего не зарегистрировано и не отправлено, публикует Ярослав.
- Каталоги: There's An AI For That, Futurepedia, AlternativeTo, Product Hunt, Toolify

## 0. Проверить до публикации

| # | Что | Почему важно | Где |
|---|---|---|---|
| 1 | Принимает ли сайт реальные оплаты Plus | В профилях стоят цены €4.99 / €10.99 / €29.99. Если Stripe ещё тестовый, цены не публикуем: ставим «Freemium» без суммы | W0-11 |
| 2 | Работает ли вход через Google и Apple | Пик трафика из Product Hunt и каталогов придётся на первые дни; со сломанным входом теряем регистрации | W0-10 |
| 3 | Что даёт бесплатный тариф: сколько планов, входит ли кошелёк билетов | Пишем только «free to start», без цифры. `[проверить вручную]` | goplanvia.com/plus |
| 4 | Открывается ли ссылка на план без регистрации | От этого зависит формулировка «share the plan with a link» и скриншот «что видит друг» | W2-02 |
| 5 | Испанская «одна фраза» | В `CLAUDE.md` она помечена как черновик, ждёт утверждения | раздел 4 |
| 6 | Платформы: только веб или есть приложения/PWA | В профилях указан только Web. Если есть приложения, добавим | продукт |

goplanvia.com с этой сессии открыть не удалось (сайт не в списке разрешённых адресов), поэтому продуктовые факты взяты только из `CLAUDE.md` и задачи.

## 1. Каталоги: цена подачи, поля, ограничения

Сайты TAAFT, Futurepedia и Toolify напрямую не открылись: адрес не в списке разрешённых или сайт вернул ошибку. Поэтому цены по ним взяты из оплатных страниц самих каталогов, где они доступны (Gumroad, /verified, /enhanced у Futurepedia), и из обзоров 2026 года. Перед оплатой Ярослав сверяет цену на странице подачи. Все источники — в разделе 6.

| Каталог | Подача | Цена (дата источника) | Что заполнить | Ограничения |
|---|---|---|---|---|
| **Product Hunt** | **Бесплатно** | Сборы в гайде не упомянуты | Name, Tagline, Description, URL, Topics, Thumbnail, Gallery, YouTube-видео, Interactive demo, Makers, Pricing, Promo, X-аккаунт, доп. ссылки, First comment, Shoutouts, дата запуска | Name ≤ 40 симв.; Tagline ≤ 60; Description ≤ 260 (Help Center) или ≤ 500 (Launch Guide), пишем ≤ 260; Topics ≤ 3; Thumbnail 240×240, < 3 МБ; Gallery 1270×760, минимум 2; без UTM и коротких ссылок; Shoutouts — 3; запуск до 1 месяца вперёд, старт в 00:01 PST |
| **AlternativeTo** | **Бесплатно**, правит сообщество | Нет | Name, описания, Platforms, License, Features (теги), категория, языки, сайт, скриншоты; альтернативы добавляются через «Suggest changes → Suggest Alternatives» на странице конкурента | Лимиты длины в FAQ не указаны. Обязательна поддержка английского; закрытые беты и приложения для одной страны обычно не принимают; модерация от пары дней до недели; рекламировать через профиль пользователя и накручивать лайки нельзя |
| **There's An AI For That** | **Платно.** Бесплатно — только ежемесячный тред в X, где выбирают один инструмент | $49 Low traffic; $347–437 Maximum Exposure (SaaSCity, 07.10.2026; OrangeBot, 19.08.2026). Nick Launches пишет «Free submission», но без даты и против двух источников 2026 года | Обязательно только URL; остальное — логотип, скриншоты, задача (task), теги, цена | На карточке в списке: название, тэглайн около 40 симв., метка задачи, метка цены («Free + from $X/mo»), дата релиза. Проверка 1–2 дня |
| **Futurepedia** | **Платно**, бесплатной подачи нет | $197 (Gumroad); $247 basic — «Sold Out»; $497 Verified (OrangeBot, 19.08.2026; futurepedia.io/verified). На /enhanced одновременно указаны $247 и $497 | URL, остальное заполняют редакторы | Карточка: короткое описание (около 60 симв.), категория, модель цены, «What is», Key features, Pros/Cons, Who is using, Pricing |
| **Toolify** | **Платно** | $99 один раз, публикация за 48 часов (mybesh, 24.05.2026; OrangeBot, 19.08.2026) | Name, Website URL, способ генерации описания (AI или вручную) | Карточка: «What is», How to use, Core features, Use cases, Pricing, FAQ. Публикуется на 10 языках |

Любая оплата — отдельное «да» Ярослава (`CLAUDE.md`, уровни одобрения). По платным каталогам ниже даны только сопоставление полей, категории и теги.

## 2. Общий набор (EN)

### 2.1. Название, сайт, подпись

- Name: **PlanVIA**
- Website: **https://goplanvia.com** (без UTM: Product Hunt не принимает ссылки с метками)
- Подпись бренда: **PlanVIA: AI Group Trip Planner**

### 2.2. Одна фраза (дословно везде)

> PlanVIA is an AI group trip planner: plan a trip with friends in minutes, with a day-by-day itinerary, a map and real places.

125 символов.

### 2.3. Тэглайн (≤ 60 символов)

| # | Тэглайн | Символов | Где лучше |
|---|---|---|---|
| A | Plan a trip with friends in minutes, with AI | 44 | Product Hunt, Futurepedia, Toolify: простой, без игры слов, как просит гайд PH |
| B | Get the trip out of the group chat and onto a map | 49 | AlternativeTo, соцсети: шутка про групповую динамику, ничего лишнего не обещает |
| C | AI group trip planner: day-by-day plans on a map | 48 | TAAFT и каталоги, где поиск идёт по категории |

Для карточки TAAFT в списке, где тэглайны около 40 символов: «AI group trip planner with day-by-day maps» (42).

### 2.4. Короткое описание (≤ 260 символов)

> PlanVIA is an AI group trip planner. Pick one of 100+ destinations and get a day-by-day itinerary with a map and real places, or copy a ready-made plan and adjust it. Share the plan with a link. Book flights, trains and hotels via partners. Free to start.

255 символов.

### 2.5. Длинное описание (120–180 слов)

Без списков: формы каталогов часто срезают разметку.

> PlanVIA is an AI group trip planner: plan a trip with friends in minutes, with a day-by-day itinerary, a map and real places.
>
> It's made for the friend who ends up organising the trip. Instead of links scattered across a group chat, you get one plan with days, places and a map, and send everyone a single link.
>
> Pick one of 100+ destinations and PlanVIA builds a day-by-day itinerary with real places on a map. Or start from the catalogue of ready-made plans: open one, copy it and adjust it for your group. Then share the plan with a link. Flights, trains, car rental, eSIM and hotels can be booked through partners (these are partner links), and bookings and tickets (PDF, images) stay in the ticket wallet. The interface is in English, Spanish, German and Russian.
>
> PlanVIA is free to start. PlanVIA Plus adds unlimited plans, an AI concierge, PDF export and offline access for €4.99/month, €10.99 for 3 months or €29.99/year.
>
> Cost splitting isn't built in: use Splitwise or Tricount alongside PlanVIA.

173 слова. Последняя строка — по ценности «честность к конкурентам». Заодно она мешает AI-ассистентам приписать нам общий бюджет.

### 2.6. Ключевые функции (8)

1. AI day-by-day itinerary with a map and real places for 100+ destinations
2. Catalogue of ready-made plans: open, copy, adjust
3. Share the plan with a link
4. Book flights, trains, car rental, eSIM and hotels through partners
5. Ticket wallet: bookings and tickets (PDF, images) in one place
6. PlanVIA Plus: unlimited plans, AI concierge, PDF export, offline access
7. Interface in English, Spanish, German and Russian
8. Free to start

Если в форме не больше 5 пунктов, берём 1, 2, 3, 4 и 6.

### 2.7. Цены

| Тариф | Цена | Что входит |
|---|---|---|
| Free | €0 | Начать бесплатно. Лимит планов — `[проверить вручную]` |
| PlanVIA Plus, месяц | €4.99 | Безлимит планов, AI concierge, PDF export, offline |
| PlanVIA Plus, 3 месяца | €10.99 | То же |
| PlanVIA Plus, год | €29.99 | То же |

Модель цены для форм: **Freemium**. В Product Hunt — **Paid (with a free trial or plan)**. Метка для TAAFT: «Free + from €4.99/mo»; если форма принимает только доллары, Ярослав решает, ставить ли пересчёт. Пробный период нигде не указываем: в списке функций его нет.

Пока не закрыт W0-11, цены не публикуем, только «Freemium».

### 2.8. Чего не пишем

- Приглашения друзей, голосования, общий бюджет, роли — этого нет. Нельзя: «invite your group», «vote», «split the budget», «plan together in real time». Можно: «plan a trip with friends», «share the plan».
- В AlternativeTo не отмечаем фичу «Real time collaboration».
- «Without sign-up» — не пишем, пока не готов W2-02.
- Стоп-слова из `CLAUDE.md` в текстах не используются (проверено поиском по файлу).

## 3. По каталогам

### 3.1. AlternativeTo — бесплатно, оформляем полностью

| Поле | Значение |
|---|---|
| Name | PlanVIA |
| Website | https://goplanvia.com |
| Short description | 2.4 |
| Description | 2.5 |
| Category | Travel & Location → Travel Planner (у Wanderlog: «Travel Planners & Travel Guides») |
| License | Freemium + Proprietary |
| Platforms | Online (Web) |
| Supported languages | English, Spanish, German, Russian |
| Features | «AI-Powered», «Works Offline» (только в Plus: в описании это есть) — эти названия есть в каталоге. Ещё 2–3 из подсказок формы: трип-планирование, itinerary, карта, бронирование. «Real time collaboration» и «Ad-free» не ставим |
| Screenshots | 3–5 штук из списка в 3.2 |

**Альтернативой каким приложениям указать** (проверено 28.10.2026):

| Приложение | Карточка на AlternativeTo | Решение |
|---|---|---|
| Wanderlog | Есть, адрес по старому названию: alternativeto.net/software/travelchime/. Категория Travel Planners & Travel Guides | **Указать** — главная цель |
| TripIt | Есть: alternativeto.net/software/tripit/, 102 альтернативы, Wanderlog среди них | **Указать**: пересечение по кошельку билетов и маршруту |
| Layla | Карточка alternativeto.net/software/layla/ — **другой продукт**: «personal AI that runs on your device», Android/iPhone, категория AI Chatbots. Это не layla.ai | **Не указывать**: попадём в альтернативы чат-боту |
| Mindtrip | Карточки не нашёл (поиск по сайту и по названию) | Не указывать. Карточки конкурентов ради ссылки на себя не создаём |
| SuperTravel (AI travel planner) | Есть: alternativeto.net/software/supertravel; в его альтернативах TripIt, Wanderlog, ChatGPT | **Предлагаю** указать как третью: прямой AI-планировщик маршрутов |

Регистрирует Ярослав со своего аккаунта и честно, как разработчик. Лайки не просим и не накручиваем: по FAQ за это понижают или удаляют карточку.

### 3.2. Product Hunt — бесплатно, оформляем полностью

| Поле | Значение | Символов |
|---|---|---|
| Name | PlanVIA | 7 |
| Tagline | Plan a trip with friends in minutes, with AI | 44 |
| Description | см. ниже | 254 |
| URL | https://goplanvia.com | — |
| Topics (до 3) | Travel, Artificial Intelligence, Productivity | — |
| Pricing | Paid (with a free trial or plan) | — |
| Makers | Ярослав (свой личный аккаунт: компании постить не могут) | — |
| X account | Нет, пока не заведены ники (W0-07) — поле пропускаем | — |
| Promo | По желанию Ярослава: скидка на Plus для сообщества PH. Только после W0-11 | — |
| Shoutouts (3, по желанию) | Lovable, Supabase — если Ярослав хочет отметить стек | — |

**Description (≤ 260):**

> PlanVIA builds a day-by-day itinerary with a map and real places for 100+ destinations, or you copy a ready-made plan and adjust it. Send the plan to friends with a link and book flights, trains and hotels via partners. Free to start, Plus from €4.99/mo.

**First comment от Ярослава (146 слов):**

> Hi Product Hunt, I'm Yaroslav, and I build PlanVIA.
>
> Most trips with friends start the same way: a group chat, a pile of links, and one person who quietly ends up doing all the planning. PlanVIA is for that person.
>
> Pick one of 100+ destinations and in a few minutes you get a day-by-day itinerary with a map and real places. Or copy a ready-made plan from the catalogue and change what doesn't fit. Then send the link to your friends. Flights, trains, hotels, car rental and eSIM can be booked through partners (those are partner links).
>
> To be upfront: it's early. Right now one person builds the plan and shares it, and there's a lot we still want to add for groups. It's free to start; Plus is €4.99/month.
>
> What does your group argue about most when planning a trip? I'd love to hear it.

Если у Ярослава есть своя история, почему он начал PlanVIA, лучше заменить ею второй абзац. Просим отзывы, а не голоса: так советует гайд PH.

**Изображения и материалы:**

| # | Что | Размер | Комментарий |
|---|---|---|---|
| 0 | Thumbnail: логотип PlanVIA | 240×240, квадрат, < 3 МБ | PNG. GIF можно, но он анимируется только при наведении |
| 1 | Главный кадр: план по дням + карта для одного города (например, Lisbon, 3 days) с подписью «A day-by-day plan with a map in minutes» | 1270×760 | Первый кадр галереи становится превью в соцсетях |
| 2 | Создание плана: выбор направления → готовый маршрут | 1270×760 | Можно склейку из двух экранов |
| 3 | Каталог готовых планов и кнопка копирования | 1270×760 | |
| 4 | Ссылка на план: что видит друг, открыв её на телефоне | 1270×760 | Только после проверки п. 4 из раздела 0 |
| 5 | Бронирование у партнёров: перелёты, поезда, авто, eSIM, отели | 1270×760 | С подписью «partner links» |
| 6 | Кошелёк билетов | 1270×760 | Только тестовые брони, без реальных имён, номеров и email |
| 7 | PlanVIA Plus: что входит и цены | 1270×760 | Только после W0-11 |
| 8 | Видео 30–60 с, запись экрана, YouTube (публичное или unlisted, полная ссылка) | — | По желанию; без AI-лиц и реальных людей |

**Когда запускать.** Product Hunt даёт один сильный запуск. Предлагаю ставить дату после W0-10 (вход) и W0-11 (оплаты), а лучше после W2-01 (совместная поездка): аудитория PH будет пробовать «group trip planner» с друзьями. Не в неделю Чёрной пятницы (27.11), когда идёт акция W4-02.

### 3.3. There's An AI For That — платно (от $49), кратко

| Поле | Значение |
|---|---|
| URL | https://goplanvia.com |
| Тэглайн на карточке | AI group trip planner with day-by-day maps (42) |
| Описание | 2.4, при длинном поле — 2.5 |
| Задача (task) | Trip planning; запасные варианты — Travel itineraries, Travel planning (выбрать из списка формы) |
| Цена | Freemium, «Free + from €4.99/mo» |
| Теги | travel, trip planner, itinerary, group travel, friends, Europe, maps |
| Медиа | Логотип и 2–3 скриншота (1, 3, 5 из 3.2) |

Бесплатно можно только откликнуться в ежемесячном треде TAAFT в X. Шанс там один из многих, сроки не предсказать.

### 3.4. Futurepedia — платно ($197–497), кратко

| Поле | Значение |
|---|---|
| Короткое описание | Day-by-day trip plans with a map for trips with friends. (56) |
| Категория | Travel |
| Модель цены | Freemium, from €4.99/mo |
| Key features | 2.6, пункты 1–4 и 6 |
| Теги | travel planning, itinerary generator, group travel, trip planner |

### 3.5. Toolify — платно ($99), кратко

| Поле | Значение |
|---|---|
| Name / URL | PlanVIA / https://goplanvia.com |
| Описание | Не генерировать AI Toolify, а вставить 2.5: иначе он додумает функции, которых у нас нет |
| Core features | 2.6 |
| Use cases | Weekend trip with friends in Europe; bachelor or bachelorette weekend; copying a ready-made city plan |
| Категории | Travel, AI Trip Planner, Itinerary Generator (выбрать из списка формы) |
| Pricing | Freemium, from €4.99/mo |

Риск у всех трёх платных каталогов один: описание «заполняют за вас» редакторы или AI. После публикации проверить, что на карточке нет голосований, общего бюджета и приглашений, а если есть — попросить исправить.

## 4. Испанские версии

**Одна фраза (ES)** — дословно из `CLAUDE.md`, черновик, ждёт утверждения Ярослава:

> PlanVIA es un planificador de viajes en grupo con IA: organiza un viaje con amigos en minutos, con un itinerario día a día, un mapa y lugares reales.

149 символов.

**Короткое описание (ES, ≤ 260):**

> PlanVIA es un planificador de viajes en grupo con IA. Elige uno de 100+ destinos y recibe un itinerario día a día con mapa y lugares reales, o copia un plan listo y ajústalo. Compártelo por enlace; reserva vuelos, trenes y hoteles con socios. Empieza gratis.

258 символов. В 260 символов «a través de nuestros socios» не помещается, поэтому «con socios». Перед публикацией текст должен проверить носитель испанского.

Испанские тексты пригодятся в AlternativeTo (если форма примет второй язык) и в будущих каталогах на испанском. Toolify переводит карточку на 10 языков сам, поэтому испанский текст стоит отправить и ему.

## 5. Что нужно от Ярослава

| # | Что | Для чего |
|---|---|---|
| 1 | Решение по платным каталогам: TAAFT (от $49), Futurepedia ($197–497), Toolify ($99). Каждая трата — отдельное «да» | 3.3–3.5 |
| 2 | Личный аккаунт Product Hunt, онбординг пройден заранее | 3.2 |
| 3 | Аккаунт AlternativeTo | 3.1 |
| 4 | Логотип: квадрат 240×240 PNG (PH) и 512×512 PNG для остальных, на прозрачном и на светлом фоне | все каталоги |
| 5 | 6–7 скриншотов 1270×760 по списку из 3.2, с тестовыми данными | PH, AlternativeTo, TAAFT |
| 6 | Видео 30–60 с на YouTube — по желанию | PH |
| 7 | Ответы на вопросы раздела 0: оплаты Plus (W0-11), вход (W0-10), лимит бесплатного тарифа, ссылка без регистрации, платформы | цены и формулировки |
| 8 | Утвердить испанскую одну фразу и короткое описание | раздел 4 |
| 9 | Выбрать тэглайн и дату запуска на PH | 2.3, 3.2 |

## 6. Источники (проверено 28.10.2026)

- Product Hunt Help Center, How to post a product — https://help.producthunt.com/posting/how-to-post-a-product
- Product Hunt Launch Guide, Preparing for launch — https://www.producthunt.com/launch/preparing-for-launch
- Пример карточки PH (темы Travel, Productivity, Android) — https://www.producthunt.com/products/venture-trip-planner
- fmerian, The anatomy of a launch plan (лимит Name 40 симв.) — https://dev.to/fmerian/the-anatomy-of-a-launch-plan-5885
- AlternativeTo FAQ — https://alternativeto.net/faq
- AlternativeTo: Wanderlog — https://alternativeto.net/software/travelchime ; TripIt — https://alternativeto.net/software/tripit/ ; SuperTravel — https://alternativeto.net/software/supertravel ; пример карточки AI Travel Planner — https://alternativeto.net/software/ai-travel-planner/about ; Layla (другой продукт), упомянута на https://alternativeto.net/software/lu
- Futurepedia: Gumroad — https://futurepedia.gumroad.com/l/submit-tool ; Verified — https://futurepedia.io/verified ; Enhanced — https://www.futurepedia.io/enhanced
- SaaSCity, обзор TAAFT (обновлён 07.10.2026) — https://saascity.io/directories/theresanaiforthat
- OrangeBot, Where to Submit Your AI Tool in 2026 (19.08.2026) — https://orangebot.ai/blog/where-to-submit-your-ai-tool-2026
- sales-theresanaiforthat ($347, проверка 1–2 дня) — https://sharedcontext.ai/skills/external/sales-skills/sales-theresanaiforthat
- Nick Launches, TAAFT («Free submission», без даты) — https://nicklaunches.com/resources/ai-directories/theresanaiforthat
- Пример карточек TAAFT в списке — https://theresanaiforthat.com/s/time-management/latest
- mybesh, Toolify ($99, обновлён 24.05.2026) — https://mybesh.com/tool/toolify
- AIPURE, Top 8 AI tools directory (12.2024, для истории цен) — https://aipure.ai/articles/top-8-ai-tools-directory
