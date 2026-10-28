# Бриф: 3 days in Lisbon with friends

- Тип: маршрут
- Язык: EN
- URL: /itineraries/3-days-in-lisbon-with-friends. Шаблон /itineraries/{маршрут} взят из документа стратегии; slug подтвердить у координатора
- Главный запрос: **3 days in Lisbon with friends**
- Для кого: 4–6 друзей 24–32 лет, бюджет средний. Летят из Великобритании, Ирландии, Германии или Нидерландов, живут в одной квартире. Интересы в группе разные: одним нужны смотровые и Синтра, другим пляж и бары
- Сезон публикации: ноябрь–декабрь 2026, под поездки март–август 2027. Пик спроса — май и июнь
- Задача в backlog: W2-05 · выдача снята 28.10.2026

## Запросы

| # | Запрос | Интент | Где спрашивают | Объём |
|---|---|---|---|---|
| 1 | 3 days in Lisbon with friends | маршрут | Google, ChatGPT | объём не проверен |
| 2 | Lisbon 3 day itinerary | маршрут | Google | объём не проверен |
| 3 | Lisbon with friends / Lisbon group trip | город, группа | Google | объём не проверен |
| 4 | how much does a 3 day trip to Lisbon cost | стоимость | Google, ChatGPT | объём не проверен |
| 5 | things to do in Lisbon with friends | идеи | Google | объём не проверен |
| 6 | where to stay in Lisbon with a group | жильё | Google | объём не проверен |
| 7 | is 3 days enough for Lisbon and Sintra | маршрут | Google, ChatGPT | объём не проверен |
| 8 | Lisbon nightlife Bairro Alto or Cais do Sodré | идеи | Google | объём не проверен |
| 9 | Lisbon in June / Santo António festival 2027 | сезон | Google | объём не проверен |
| 10 | is the Santa Justa lift open | факт | Google | объём не проверен |
| 11 | Lisbon stag weekend / Lisbon hen do | сегмент | Google | объём не проверен |
| 12 | «Plan 3 days in Lisbon for 5 friends in May, about €350 each without flights» | маршрут, разговорный | ChatGPT | объём не проверен |
| 13 | «We're 6 friends, half want Sintra and half want the beach — how do we split a Lisbon trip?» | группа, разговорный | ChatGPT | объём не проверен |

Пересекается с промптами AI-замера `en-09` и `es-06` из `data/ai-visibility-prompts.csv`.

## Вопросы для H2

Структура по шаблону «Страница города» из `templates/pages.md`, дни идут отдельными H2.

1. **How much do 3 days in Lisbon cost for 4 friends?** Сначала итог на человека без перелётов, потом таблица. Отдельной строкой — туристический сбор на человека за ночь.
2. **Where should a group of 4–6 stay in Lisbon?** Сравнить Baixa/Chiado, Cais do Sodré и Alfama: подъёмы с чемоданами, шум баров ночью, от скольких спален реально найти квартиру на 6.
3. **Which Lisbon lifts and funiculars are running in 2027?** Это главный козырь: конкуренты до сих пор водят через закрытые подъёмники, подробности в «Что в выдаче». Нужен ответ «что вместо», с ценой одной XL-машины на 6 против шести билетов.
4. **Is 3 days enough for Lisbon and Sintra with a group?** Время на поезде, билеты в Pena на сеанс, как разделить группу на день по правилу 70/30.
5. **When is the best time for a group trip to Lisbon in 2027?** Пиковые даты 2027 с днями недели (см. «Факты»): ночь Santo António с субботы 12 на воскресенье 13 июня, праздники 25 апреля, 1 мая, 27 мая (Corpus Christi), 10 июня. Честно про жару и толпы в июле–августе.

**Дни (H2), черновик логики, места и порядок уточнит автор:**
- Day 1: Baixa → Alfama → Graça. Наверх едем, вниз идём пешком через смотровые. Вечер — Bairro Alto или Cais do Sodré.
- Day 2: Belém и LX Factory. **Не в понедельник**: проверить выходные дни Jerónimos и Torre de Belém.
- Day 3: один день на два маршрута по правилу 70/30. Часть группы едет в Синтру, часть — на пляж в Cascais или Carcavelos по линии с Cais do Sodré. Вечером встречаемся за общим ужином.

**Именованное правило PlanVIA** (выбрать одно):
- **Up by ride, down on foot.** На холмы Лиссабона группа из 6 поднимается одной машиной и делит счёт, а вниз идёт пешком через смотровые. Работает, только если в тексте будет проверенное сравнение цены.
- **70/30** на день 3, как сквозное правило всех страниц.

**Цитата практика:** гид по Лиссабону, который водит группы, или организатор мальчишников и девичников в Лиссабоне.

## Что в таблице с цифрами

Считаем на человека, два столбца: группа из 4 и группа из 6.

| Строка | Per person (4) | Per person (6) | Source | Checked |
|---|---|---|---|---|
| Квартира, 3 ночи | | | выборка Booking и Airbnb на конкретные даты мая 2027, с датой снимка; это ориентир, а не цена места | Nov 2026 |
| Туристический сбор, 3 ночи | | | lisboa.pt | |
| Из аэропорта в город: метро или одна машина на группу | | | metrolisboa.pt; оценка Bolt/Uber в приложении с датой | |
| Транспорт по городу: navegante или Lisboa Card 72h | | | carris.pt, metrolisboa.pt, visitlisboa.com | |
| Belém: Jerónimos + Torre de Belém | | | museusemonumentos.pt | |
| Синтра: поезд туда-обратно + один дворец | | | cp.pt, parquesdesintra.pt | |
| Еда, 3 дня, средний уровень | | | выборка меню с официальных сайтов 3–4 мест | |
| Вечер в барах | | | ориентир, помечается как оценка | |
| **Итого без перелётов** | ~€… | ~€… | | |

## Факты, которые надо проверить

| Факт | Где проверять |
|---|---|
| Туристический сбор: сколько € за ночь с человека, максимум ночей, льготы по возрасту. По СМИ, €4 с сентября 2024 — не проверено | lisboa.pt (Taxa Municipal Turística) |
| Статус подъёмников. RFM от 02.09.2026 пишет: Glória закрыт, новую установку ждут в 1-й половине 2029; Bica, Lavra и Santa Justa закрыты без даты открытия; Graça работает с 30.04.2026. Пока это «reported, not confirmed» | carris.pt; ещё раз проверить перед публикацией |
| Трамвай 28: цена билета на борту и через navegante или Zapping | carris.pt |
| Тарифы метро, суточный билет, Zapping, линия из аэропорта и время в пути | metrolisboa.pt, navegante.pt |
| Lisboa Card 24/48/72h: цены и что входит (поезд до Синтры и Кашкайша, музеи) | visitlisboa.com (Turismo de Lisboa) |
| Jerónimos и Torre de Belém: цены, выходные, нужен ли билет на сеанс | museusemonumentos.pt (Museus e Monumentos de Portugal) |
| Castelo de São Jorge: цена, часы | castelodesaojorge.pt |
| Синтра: билеты в Pena на сеанс, цены дворцов, шаттл-автобус, ограничения движения для машин и тук-туков | parquesdesintra.pt; cm-sintra.pt |
| Поезда Rossio–Sintra и Cais do Sodré–Cascais: время, цена, интервал | cp.pt |
| Time Out Market и LX Factory: часы | timeoutmarket.com/lisboa; lxfactory.com |
| Праздники Португалии 2027: 25 апреля, 1 мая, Corpus Christi 27 мая, 10 июня; муниципальный праздник Лиссабона 13 июня | официальный календарь (diariodarepublica.pt, gov.pt); lisboa.pt |
| Festas de Lisboa 2027: даты и места arraiais | festasdelisboa.com / egeac.pt |
| NOS Alive 2027: даты. Проверить, есть ли в 2027 Rock in Rio Lisboa (фестиваль не ежегодный) | nosalive.com; rockinriolisboa.pt |
| Климат май–август: температура воздуха и воды | ipma.pt (normais climatológicas) |
| Бронь столиков на 6 человек в упомянутых ресторанах | официальные сайты ресторанов |
| EES и ETIAS для приезжающих из Великобритании | travel-europe.europa.eu; ссылка на нашу /travel-alerts |

## Что в выдаче и AI-ответах сейчас

Выдачу смотрел через WebSearch 28.10.2026 (индекс США, это не Google напрямую). Ответы AI-ассистентов не проверены, W1-04 заблокирован.

- **[TripProf — «3 Days in Lisbon With Friends: A Route That Actually Fits»](https://tripprof.com/en/itineraries/3-days-in-lisbon/)** — прямой конкурент с тем же углом. Обновлена 18.07.2026, есть копии на 8+ языках, в том числе /es/. Минусы: 28 остановок за 3 дня, «~€92 per person» без разбивки и без источников, все 5 ответов в FAQ пустые (включая «Is the funicular to Bairro Alto running again?» и «how to split costs»), дни недели не учтены. Плюс: есть советы для групп (столик на фаду бронировать за 2–3 дня, групповые туры от 4 человек).
- **[Layla — «3-Day Lisbon City Break with Friends»](https://layla.ai/trip/3-day-lisbon-city-break-with-friends/01JSMNYJMDFGSZBZSSXEAJJJ48)** — AI-сгенерированная страница поездки. В заголовке 3 дня, а внутри 4. Тур в Синтру на 9,5 часа стоит в день прилёта. Нет ни одной цены, нет часов работы. В маршруте Santa Justa Lift, который закрыт с сентября 2025 (по RFM). Советов для группы нет, только «3 travellers».
- **[Earth Trekkers — «3 Days in Lisbon»](https://www.earthtrekkers.com/3-days-in-lisbon-itinerary/)** — сильная классика, обновлена 02.12.2025. Подробные советы по очередям, два варианта: Лиссабон целиком и Лиссабон + Синтра. В маршруте Santa Justa Lift и фуникулёр Bica — оба закрыты (по RFM). Цена на человека не посчитана. Для группы ничего нет: ни ночной жизни, ни жилья на 6, ни того, как делиться.

**Чего не хватает группе:** цены на человека для 4 и для 6; актуальных данных по подъёмникам; логики дней недели (понедельник в Belém); жилья для компании; решения «половина хочет в Синтру, половина на пляж»; вечеров.

## Угол PlanVIA

**Лиссабон для компании, проверенный на 2027 год.** Цена на человека для 4 и 6 друзей с источниками и пометкой «Checked: Nov 2026». Честно о том, что закрыто: подъёмники Santa Justa, Glória и Bica, по которым до сих пор водят конкуренты. Дни расставлены с учётом выходных. День 3 делится по правилу 70/30, вечером общий ужин. План копируется в PlanVIA одной кнопкой.

Не обещаем: голосование за день в Синтре, общий бюджет, приглашения. Пишем «share the plan with your group».

## Маршрут или шаблон PlanVIA

<план из каталога: уточнить у координатора>

Нужен план «Lisbon, 3 days» из каталога, или его надо создать и поправить под логику дней из этого брифа: без закрытых подъёмников, Belém не в понедельник, день 3 на два маршрута.

## Метаданные (черновик)

- Title (60 символов): `3 Days in Lisbon with Friends: Itinerary and Costs | PlanVIA`
- Description (134 символа): `3 days in Lisbon for 4–6 friends: day-by-day route, map, cost per person and which historic lifts are closed. Prices checked Nov 2026.`
- Заголовок превью: `3 days in Lisbon with friends`
- Подзаголовок превью: `Itinerary, map and costs for your group`

## Заметки координатору

- Статус подъёмников годится и как запись для /travel-alerts. Предложено в `plan/backlog.md` → «Идеи».
- TripProf — прямой конкурент: /itineraries/ «with friends» на многих языках плюс подборки «best group travel planning apps». Стоит добавить в список сравнений (W3-04) и в мониторинг AI-замера.
