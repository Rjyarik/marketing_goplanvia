# Бриф: хаб «AI trip planner for friends»

- Тип: хаб
- Язык: EN. ES-версию готовим отдельно, это адаптация под испанский рынок, а не перевод (W2-03)
- URL: /plan/friends-trip-planner. Перед публикацией разработчик проверяет роутинг, см. «Риски», п. 1
- Главный запрос: **trip planner for friends**. Ядро кластера: «AI trip planner for friends», «AI group trip planner»
- Для кого: компания из 4–8 друзей 22–33 лет, едут по Европе на 2–4 дня, бюджеты разные. Планирует обычно один человек, который устал вести всё в чате
- Сезон публикации: ноябрь 2026 (W2-03). Страница вечнозелёная, а поездки в таблице подбираем под весну и лето 2027
- Задача в backlog: W2-03 · выдача снята 28.10.2026

## Запросы

Объём ни по одному запросу не проверен: Search Console и BabyLoveGrowth ещё не подключены (W0-02, W0-06).

| # | Запрос | Интент | Где спрашивают | Объём |
|---|---|---|---|---|
| 1 | trip planner for friends | категория, коммерческий | Google | объём не проверен |
| 2 | AI trip planner for friends | категория | Google, ChatGPT | объём не проверен |
| 3 | AI group trip planner | категория | Google, ChatGPT | объём не проверен |
| 4 | group trip planner app | категория | Google | объём не проверен |
| 5 | best app to plan a trip with friends | сравнение | Google, ChatGPT | объём не проверен |
| 6 | collaborative trip planner | категория | Google | объём не проверен |
| 7 | free group trip itinerary planner | категория | Google | объём не проверен |
| 8 | how to plan a trip with friends | how-to | Google, ChatGPT | объём не проверен |
| 9 | how far in advance should you plan a group trip | how-to | Google, ChatGPT | объём не проверен |
| 10 | trip planner app where friends can plan together | категория | ChatGPT | объём не проверен |
| 11 | «What's the best app to plan a 3-day trip in Europe with 5 friends?» | сравнение, разговорный | ChatGPT, Perplexity | объём не проверен |
| 12 | «Can AI make one itinerary for 6 friends with different budgets?» | категория, разговорный | ChatGPT | объём не проверен |
| 13 | Wanderlog vs Layla for a group trip | сравнение | Google, ChatGPT | объём не проверен |

Эти запросы пересекаются с промптами AI-замера `en-01, en-02, en-03, en-08, en-13, en-17, en-18` из `data/ai-visibility-prompts.csv`. Когда аналитик снимет базовый замер (W1-04), сверить, кого AI-ассистенты называют по этим промптам.

## Вопросы для H2

1. **How do you plan a trip with friends without the group chat taking over?** Метод из 4 шагов, у каждого шага цифра: потолок трат на человека, два варианта дат, шорт-лист из трёх городов, один человек собирает план и делится ссылкой. PlanVIA закрывает последний шаг: маршрут по дням с картой за минуты, потом «share the plan». Голосования, общего бюджета и ролей в тексте нет: договариваться группа будет вне продукта.
2. **What does an AI trip planner actually do for a group trip, and what doesn't it?** Сначала то, что есть: маршрут по дням, карта, реальные места, 100+ направлений, каталог готовых планов, бронирование у партнёров. Потом честно, чего нет: делить расходы помогут Splitwise или Tricount, чат остаётся в WhatsApp.
3. **How much does a 3-day trip with friends in Europe cost per person?** Ответ в одном предложении с вилкой из таблицы ниже. Цифры берём только со страниц городов, которые уже прошли фактчек.
4. **How far ahead should a group of friends start planning?** Ответ с цифрами: за сколько месяцев брать перелёты и за сколько дней — билеты на сеанс (Pena в Синтре, Torre de Belém). Отдельно пиковые даты 2027: Semana Santa 21–28 марта, Santo António в Лиссабоне в ночь на 13 июня.
5. **Which apps should your group use for what?** Таблица задач: маршрут — PlanVIA, совместное редактирование — Wanderlog, расходы — Splitwise или Tricount, чат — WhatsApp. Обязательная строка «When to choose another tool instead» — это требование ценности «честность к конкурентам».

**FAQ (H3)**, вопросы взяты из документа стратегии и адаптированы под то, что есть в продукте:
- Is PlanVIA free? (бесплатный план и что даёт Plus, цена со страницы /plus)
- How do I share my trip plan with friends? (описываем только реальный способ, см. «Факты»)
- Which cities can I plan with PlanVIA?
- Can we book flights, trains and hotels in PlanVIA? (раскрываем, что это партнёрские ссылки)
- How do you split costs on a group trip? (честный ответ: внешним приложением)
- What if someone drops out? (совет про невозвратные брони и депозиты, без функций продукта)

**Именованное правило PlanVIA** (выбрать одно, согласовать с координатором):
- **Cap before city.** Сначала группа договаривается о потолке трат на человека без перелётов, и только потом кто-то предлагает город.
- **70/30.** 70% программы проводим вместе, 30% каждый как хочет. Пример из `CLAUDE.md`, его стоит сделать сквозным правилом для всех страниц.

**Цитата практика:** организатор групповых поездок или координатор студенческих поездок. Нужен реальный человек, искать через outreach.

## Что в таблице с цифрами

**Таблица 1. «Ready-made trips with friends»** — главная таблица хаба.
- Строки: 4–6 планов из каталога, у которых уже есть проверенная страница города или маршрута. Первые — Lisbon 3 days и Porto 4 days (см. соседние брифы от 29.10).
- Столбцы: City · Days · Built for (group size) · Est. per person, excl. flights (€) · Biggest cost item · Checked · Copy this itinerary.
- Считаем на человека, для группы из 4 человек в одной квартире. Цифры только из опубликованных проверенных страниц. Пока таких страниц меньше трёх, в таблицу идут только готовые строки.

**Таблица 2. «Which tool for which job»** — без цен, если только цены не сняты со страниц продуктов с датой.
- Столбцы: Task · PlanVIA · Other tool · Why.
- Строки: day-by-day itinerary, map of real places, booking, editing together, splitting costs, group chat.

## Факты, которые надо проверить

| Факт | Где проверять |
|---|---|
| Что есть в продукте: 100+ направлений, 4 языка интерфейса, партнёры (перелёты, поезда, авто, eSIM, отели) | `CLAUDE.md`, раздел «Продукт: что есть сейчас»; goplanvia.com/releases |
| Что входит в PlanVIA Plus и сколько стоит | goplanvia.com/plus |
| Как сейчас работает «share the plan»: ссылка, только просмотр или с регистрацией | сам продукт; уточнить у координатора |
| Открывается ли план из каталога без регистрации и есть ли «Copy trip» | goplanvia.com/plans; статус W2-02 в `plan/backlog.md` |
| Цена на человека для каждой строки таблицы 1 | опубликованные страницы городов; `data/place-facts.csv` |
| За сколько месяцев брать перелёты | первоисточник исследования: отчёт Google Flights или Expedia/ARC Air Travel Hacks. Going (going.com) — только вторичный источник |
| За сколько дней раскупают сеансы в Pena и Torre de Belém | parquesdesintra.pt; museusemonumentos.pt |
| Возможности конкурентов в таблице 2: совместное редактирование и раздел расходов у Wanderlog, AI-чат у Layla | wanderlog.com, layla.ai — страницы продуктов, с датой проверки |
| Что бесплатно в Splitwise и Tricount | splitwise.com, tricount.com |
| Даты Semana Santa 2027 и Santo António 2027 | BOE (fiestas laborales 2027); lisboa.pt / festasdelisboa.com |
| Текст раскрытия партнёрских ссылок | координатор |

## Что в выдаче и AI-ответах сейчас

Выдачу смотрел через WebSearch 28.10.2026. Это не Google напрямую (индекс США), поэтому позиции ориентировочные. Ответы ChatGPT и Perplexity не проверены: AI-замер заблокирован (W1-04), Search Console не подключена.

В топе три типа страниц:

1. **Лендинги продуктов.** [Pilot — /group-trip-planner](https://www.pilotplans.com/group-trip-planner), title «Free Group Trip Planner App: One Shared Plan | Pilot». Сильные стороны: социальное доказательство (50,000+ groups, рейтинг 4.7) и FAQ из 11 вопросов. Совместное редактирование есть, голосования и деления расходов на странице нет, готовых маршрутов на выходные тоже нет. Второй образец — [Layla — /plan/couple-trip-planner](https://layla.ai/plan/couple-trip-planner), сегментный шаблон, с которого в стратегии скопирована схема /plan/…. Сегмент «пары» есть только в title и подсказках чата, FAQ общий, реальных маршрутов на странице нет. Страницу Layla для друзей или групп в выдаче не нашёл.
2. **Подборки «best group travel apps».** [TripIt Blog](https://www.tripit.com/web/blog/travel-tips/best-group-travel-planning-app) от 21.01.2026 советует TripIt, WhatsApp, Splitwise, Venmo и PackPoint; AI-планировщиков там нет. Вокруг много подборок «best group trip planning apps 2026» на *.pages.dev от мелких конкурентов (nomadcrew, tripsquad, tripprof). Похоже на масштабированный контент, но AI-ответы такие подборки могут цитировать.
3. **How-to гайды.** [Going — «How To Plan A Trip With Friends: 12 Practical Tips!»](https://www.going.com/guides/how-to-plan-a-trip-with-friends) от 09.03.2026. Советы общие, пунктов 8 и 9 на странице нет. Нет ни примера маршрута, ни цен на человека. Из инструментов советуют Kayak Trip Huddle, Splitwise и Tricount.

**Чего не хватает группе.** Ни одна страница не даёт вместе три вещи: (а) готовый маршрут по дням, (б) цену на человека для компании и (в) честный ответ, каким инструментом делать какую часть. Лендинги AI-продуктов не показывают ни одного настоящего маршрута, а гайды не дают инструмента, который этот маршрут соберёт.

## Угол PlanVIA

**Показать, а не рассказать.** Хаб работает как витрина настоящих готовых поездок с друзьями: у каждой цена на человека с датой проверки и кнопка «Copy this itinerary». Рядом стоят метод «как договориться» (советы, а не функции) и честная таблица «какой инструмент для чего».

- Фраза о продукте при первом упоминании — дословно: *PlanVIA is an AI group trip planner: plan a trip with friends in minutes, with a day-by-day itinerary, a map and real places.*
- Можно писать: «plan with friends», «share the plan», «copy this itinerary».
- Нельзя писать: «vote», «split the budget», «invite your group», «group agrees in one evening». Позиционирование «договориться за вечер» ждёт выпуска совместной поездки (W2-01).
- Финал страницы — «Copy this itinerary» или «Create a trip», но не «Sign up».

## Маршрут или шаблон PlanVIA

<план из каталога: уточнить у координатора>

Для таблицы 1 нужно 4–6 планов. Первыми идут Lisbon 3 days with friends и Porto, Semana Santa 4 days (см. соседние брифы).

## Метаданные (черновик)

- Title (56 символов): `AI Trip Planner for Friends: Plan a Group Trip | PlanVIA`
- Description (142 символа): `Plan a trip with friends in minutes: a day-by-day itinerary, a map and real places for 100+ destinations. Share the plan or copy a ready trip.`
- Заголовок превью: `Plan a trip with friends in minutes`
- Подзаголовок превью: `Day-by-day itinerary, map and real places`

## Риски и вопросы координатору

1. **Возможный конфликт роутинга.** Готовые планы живут на /plan/{id} (документ стратегии, «Сайт», раздел 1). Адрес /plan/friends-trip-planner может уйти в этот же маршрут как id плана и отдать 404 или пустой план. Нужна проверка разработчика: либо явный приоритет статического маршрута, либо другой адрес, например /friends-trip-planner.
2. **Документ стратегии расходится с `CLAUDE.md`.** Во вкладке «Сайт: страницы и заголовки» у хаба description «Agree on dates, budget and daily plans in one shared trip» и H2 «Pick dates everyone can make», «Agree on a budget…», «Share the work: who books, who pays deposits». Всё это обещает функции, которых пока нет. Предлагаю до W2-01 оставить H2 из этого брифа, а версию из документа вернуть после выпуска совместной поездки.
3. **Написание бренда.** В той же вкладке title заканчивается на «| PlanVia», в `CLAUDE.md` правило — только PlanVIA. В брифе везде PlanVIA, документ надо поправить.
4. **«Copy without sign-up» зависит от W2-02.** Пока кнопка не работает без регистрации, автор не обещает «no sign-up».
