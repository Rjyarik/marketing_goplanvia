# Фактчек: зимние ролики (ярмарки, Новый год в Вене, лыжи в Zillertal Arena), EN + ES

Черновик: `content/social/2026-10-30-winter-video-scripts.md` (задачи W3-02 / W3-03), строки `data/place-facts.csv` 124–140 (checked_by=social-producer, 2026-10-30).
Фактчекер, проверено 2026-10-30. Каждую цифру сверял с открытой страницей или PDF; сниппеты поиска как источник не брал. Текст черновика не менял, ниже только «что на что заменить». L62 = строка 62 черновика.
Правила о продукте взяты из обновлённого `CLAUDE.md` (раздел «Продукт: что есть сейчас», строки 21–33, «со слов Ярослава, 30.10.2026»): теперь можно писать invite your friends / vote / chat with your group / keep everyone's tickets in one place, по-прежнему нельзя split the budget / track who owes what.

Вердикт: **пропускаю после правок** (правка нужна только в v2).

## Итог по роликам

| Ролик | Итог | Можно нести Ярославу | Что мешает |
|---|---|---|---|
| **v1-christmas-markets** (окно 2–6 нояб.) | **pass** | **Да, сейчас.** | Ничего. Все 13 фактов совпали с wien.info и nuernberg.de. При одобрении Ярославу нужно ответить на вопрос 2: есть ли Вена и Нюрнберг среди 100+ направлений (см. «Утверждения о продукте»). |
| **v2-nye-vienna** (окно 16–27 нояб.) | **fix** | После одной правки. | Правило 70/30 искажено (п. 21). Все даты, часы и правила совпали со страницей 2026/27, перепроверять их после правки не нужно. |
| **v3-ski-zillertal** (окно 9–13 нояб.) | **pass** | **Да.** | Цены, сезон, групповая скидка и арифметика верны. Условие то же, что у v1: вопрос 2, есть ли Zell am Ziller среди направлений. Если нет, заменить одну фразу (п. 38). Есть рекомендации по точности (п. 33, 35), и цены нужно перепроверить накануне публикации. |

| | Всего | pass | fix | cannot verify |
|---|---|---|---|---|
| Проверяемые утверждения | 40 | 37 | 1 | 2 |

«Cannot verify» относится только к продукту: покрытие направлений (п. 38) и ES-фраза о продукте, которая ждёт утверждения Ярослава (п. 39). Внешних фактов без подтверждения нет.

**Как проверял.** WebFetch выдаёт пересказ страницы, поэтому у каждой страницы просил дословные цитаты, а каждую цифру сверял минимум по двум официальным страницам или PDF. Пересказы между собой сошлись. Исключение одно: к какому ски-пассу относится «4 in 6» (п. 35).

## Таблица утверждений

### v1-christmas-markets: проверено первым

| # | Утверждение | Источник | Проверено | Вердикт | Что заменить |
|---|---|---|---|---|---|
| 1 | Вена, Rathausplatz: 13 нояб. – 26 дек. 2026 (L45, L62, L73, L92, L103) | https://www.wien.info/en/now-on/christmas/christmas-markets-342664: «Nov 13 – Dec 26, 2026» | 2026-10-30 | верно | — В таблицах и CSV ссылку давать без `?pp=1`: каноничный URL отдаёт то же |
| 2 | Вена: ежедневно 10:00–22:00 (L62, L73, L92, L103) | там же: «Daily from 10am to 10pm»; PDF организатора: «täglich von 10:00 bis 22:00 Uhr» | 2026-10-30 | верно | — |
| 3 | Вена, 24 дек.: закрытие в 18:30 (L65, L95) | там же: «Dec 24, 10 am to 6.30 pm»; PDF: «24.12.2026: 10:00 – 18:30 Uhr» | 2026-10-30 | верно | Необязательно: в EN/ES-подписи (L73, L103) про 18:30 не сказано, хотя в ролике сказано |
| 4 | Вена: 44 рабочих дня (L45, только таблица) | https://www.christkindlmarkt.at/wp-content/uploads/2026/01/01_Wiener-Christkindlmarkt-2026_Information-Standbewerbung.pdf: «Marktzeitraum: 13.11.2026 – 26.12.2026 (entspricht 44 Betriebstage)»; по календарю 18 + 26 = 44 | 2026-10-30 | верно | — Документ рассчитан на участников (приём заявок 19.01–19.03.2026), для зрителя источник — wien.info |
| 5 | Нюрнберг открывается в пятницу 27 нояб. 2026, церемония в 17:30 (L46, L63, L73, L93, L103) | https://www.nuernberg.de/internet/kommunikation_stadtmarketing_en/christmas_market.html: «Friday, November 27, 2026, at 5.30 pm»; EN-PDF ckm_26_information_en.pdf; Ausblick: «Freitag, 27. November 2026, um 17.30 Uhr» | 2026-10-30 | верно | — |
| 6 | Нюрнберг работает до 24 дек. (L46) | https://www.nuernberg.de/internet/stadtportal/christkindlesmarkt.html: «vom 27. November bis 24. Dezember» (раздел «Termin 2026») | 2026-10-30 | верно | — |
| 7 | Нюрнберг: ежедневно 10:00–21:00 (L47, L63, L93) | портал: «täglich von 10 bis 21 Uhr»; EN-PDF: «From Saturday, November 28, to Wednesday, December 23, from 10 am to 9 pm» | 2026-10-30 | верно | — |
| 8 | Нюрнберг, день открытия: до 22:00, пауза 17:30–18:00 (L47, только таблица) | портал: «von 17.30 bis 18 Uhr unterbrochen», «bis 22 Uhr geöffnet» (Lange Nacht); EN-PDF: «Friday, November 27, 2026, from 10 am to 10 pm» | 2026-10-30 | верно | — |
| 9 | Нюрнберг, 24 дек.: закрытие в 14:00 (L65, L73, L95, L103) | портал: «Am 24. Dezember endet der Markt um 14 Uhr»; EN-PDF: «Thursday, December 24, … from 10 am to 2 pm» | 2026-10-30 | верно | — |
| 10 | «up to 180 stalls» / «hasta 180 puestos» (L48, L63, L93) | https://www.nuernberg.de/imperia/md/kommunikation_stadtmarketing/dokumente/internet/ckm/ckm_26_ausblick.pdf: «bis zu 180 Buden mit rot-weißen Stoffdächern» (в EN-PDF «approximately 180 stalls») | 2026-10-30 | верно | — |
| 11 | Полных выходных внутри дат: Вена 6, Нюрнберг 4 (L49, L64, L73, L94, L103) | Свой расчёт по календарю 2026: 13.11 — пт, 26.12 — сб, 27.11 — пт, 24.12 — чт. Вена: 14–15, 21–22, 28–29 нояб.; 5–6, 12–13, 19–20 дек. = 6 (26.12 — суббота без воскресенья). Нюрнберг: 28–29 нояб.; 5–6, 12–13, 19–20 дек. = 4 | 2026-10-30 | верно | — |
| 12 | Цен (вход, залог за кружку, глинтвейн) в ролике нет (L50) | wien.info: на странице нет ни платы за вход, ни залога, ни цен | 2026-10-30 | верно | — Для будущих роликов цены остаются `[проверить вручную]` |
| 13 | Окно 2–6 нояб.: Вена открывается 13 нояб. (L12) | п. 1 | 2026-10-30 | верно | — |

### v2-nye-vienna

| # | Утверждение | Источник | Проверено | Вердикт | Что заменить |
|---|---|---|---|---|---|
| 14 | Silvesterpfad 31 дек. 2026, 14:00–02:00 (L156, L163, L174, L186, L193, L204) | https://www.wien.info/en/now-on/christmas/new-years-eve-354224: «December 31, 2026», «From 2.00 pm in the afternoon to 2.00 am the following morning»; DE https://www.wien.info/de/aktuell/weihnachten/silvester-358870: «31.12.2026», «14-2 Uhr» | 2026-10-30 | верно | — DE-ссылка из черновика `/de/musik-buehne/silvester-358870` перенаправляет на этот URL, лучше давать его |
| 15 | Вход свободный (L156, L163, L174, L186, L193, L204) | EN: «eight locations with free admission»; DE: «bei freiem Eintritt» | 2026-10-30 | верно | — |
| 16 | Еда и напитки с 11:00 (L144, только таблица) | EN: «from 11.00 am»; DE: «Gastronomie ab 11 Uhr» | 2026-10-30 | верно | — |
| 17 | В полночь звонит Pummerin в соборе св. Стефана и звучит «Голубой Дунай» (L174, L204) | EN: «the Pummerin, the famous bell in St. Stephen's Cathedral», «Blue Danube Waltz»; DE: «Donauwalzers und der Pummerin» | 2026-10-30 | верно | — |
| 18 | Ракеты и петарды (от F2) запрещены во всей Вене (L166, L174, L196, L204) | EN: «rockets and firecrackers (from category F2) are prohibited throughout Vienna»; DE: «Zünden von Raketen und Knallkörpern (ab Kategorie F2) in ganz Wien verboten» | 2026-10-30 | верно | — |
| 19 | Каток у Ратуши 31 дек. закрыт; сезон 13.11.2026 – 06.01.2027 (L147, L166, L174, L196, L204) | wien.info (страница ярмарок), Vienna Ice World: «Nov 13, 2026 – Jan 6, 2027», «Dec 31: closed» | 2026-10-30 | верно | — |
| 20 | Новогодний концерт 1 янв. 2027 с 11:15, экраны на Stephansplatz (L165, L174, L195, L204) | EN: «January 1, 2027, starting at 11:15 am», «Stephansplatz and Riesenradplatz in the Prater»; DE: «am 1.1.2027 ab 11.15 Uhr» | 2026-10-30 | верно | — Что трансляция бесплатная, на странице не сказано. В ролике этого нет, так и оставить |
| 21 | **«Our 70/30 rule: midnight together, the rest is free choice»** (L165 титр и голос, L174 подпись, L195, L204) | `CLAUDE.md` L83: «70/30: 70% программы общие, 30% каждый проводит как хочет»; LinkedIn c1 (`content/social/2026-10-30-linkedin-posts.md` L19–20): «70% of the trip is shared… 30% is free» | 2026-10-30 | **неверно** | Правило перевёрнуто: общая только полночь, остальное свободно, то есть почти 0/100. Заменить, чтобы общей была большая часть ночи. EN, титр: `70/30` / `70% together: dinner + midnight · 30% your call`; голос: «Our 70/30 rule: dinner and midnight together, the rest of the night is your call.»; подпись L174: «(our 70/30 rule: dinner and midnight together, the rest of the night is your call)». ES, титр: `70% juntos: cena + medianoche · 30%, a tu aire`; голос: «Regla 70/30: cena y medianoche juntos; el resto de la noche, a vuestro aire.»; подпись L204: «(nuestra regla 70/30: cena y medianoche juntos; el resto de la noche, a vuestro aire)». Хронометраж ES проверить при записи |
| 22 | Число локаций Silvesterpfad в ролике не используется (L151) | EN: страница пишет «eight locations», но полного списка из восьми не даёт: маршрут Freyung – Am Hof – Graben – Stephansplatz – Kärntner Straße – Neuer Markt, плюс Rathausplatz и Prater/Riesenradplatz | 2026-10-30 | верно (что не используем) | — У автора «в карточках пять»; число и дальше не использовать |

### v3-ski-zillertal

| # | Утверждение | Источник | Проверено | Вердикт | Что заменить |
|---|---|---|---|---|---|
| 23 | Цены сезона 2026/27 (L242, L264, L275) | https://www.zillertalarena.com/en/zell/winter/ski-pass-prices/: заголовок «Zillertal Arena Ski Pass Prices 2026–27» | 2026-10-30 | верно | — |
| 24 | Взрослый дневной билет с 8:00: €82 (L264, L265, L275, L294, L305) | там же и https://www.zillertalarena.com/en/winter/ski-area/tickets-prices/: «from 8.00/8.30/9.00 a.m.» € 82,00; групповой PDF: 82,00 | 2026-10-30 | верно | — |
| 25 | С 10:30: €78,50 | обе страницы и PDF: € 78,50 (только в кассе, «cash desk only») | 2026-10-30 | верно | — |
| 26 | С 12:00: €63,50 | обе страницы и PDF: € 63,50 (только в кассе) | 2026-10-30 | верно | — |
| 27 | С 13:30: €45 | обе страницы и PDF: € 45,00 (только в кассе) | 2026-10-30 | верно | — |
| 28 | Сезон 4 дек. 2026 – 11 апр. 2027, «snow permitting» (L264, L275, L294, L305) | обе страницы: «04.12. - 11.04.2027 (with sufficient snow)»; group-offer: «the season may start later or end earlier than stated» | 2026-10-30 | верно | — |
| 29 | «Prices may be subject to change» → «may change» в подписи (L246, L277, L307) | обе страницы: «Prices may be subject to change» | 2026-10-30 | верно | — Окно публикации 9–13 нояб.: цены перепроверить накануне |
| 30 | 6 × €82 = €492 (L265, L275, L295, L305) | арифметика | 2026-10-30 | верно | — |
| 31 | 2 × 82 + 2 × 78,50 + 2 × 45 = 164 + 157 + 90 = €411; разница с €492 = €81 (L248, L265, L275) | арифметика | 2026-10-30 | верно | — |
| 32 | «Joins after lunch? −€37»: 82 − 45 = 37 (L265, L295) | арифметика | 2026-10-30 | верно | — |
| 33 | Групповая скидка 10% от 11 человек (L266, L275, L296, L305) | group-offer: «For groups of 11 or more, you will receive a 10% discount», только «1 or 1.5 days ski pass, valid only for the Zillertal Arena»; PDF: «ski passes must be purchased by 1 person» | 2026-10-30 | верно | Рекомендация, не обязательно: в подписи L275 «Group discount starts at 11 people (10%)» дописать «on 1-day Arena passes bought together» (ES L305: «en forfaits de 1 día comprados juntos») |
| 34 | «Six of you: full price» (L266, L296) | порог 11 (п. 33); PDF: «No student or senior citizen discounts are offered in the entire Zillertal» | 2026-10-30 | верно | — |
| 35 | Билет «4 in 6»: €317,50, 4 дня катания на выбор в пределах 6 (L243, L267, L275, L297, L305) | https://www.zillertalarena.com/en/winter/ski-area/tickets-prices/: раздел «Elective tickets», «4 in 6» € 317,50, «Ski whenever you like within the given days»; https://www.zillertal.at/en/winter/holidays/zillertal-superskipass.html: «flexipass 4 in 6» € 317,50 в тарифах Zillertaler Superskipass 2026/2027 | 2026-10-30 | верно (цена и условие) | Рекомендация. Источники расходятся в том, чей это билет. На zillertalarena.com раздел идёт после Superskipass и зона не указана, а из билетов только для Арены многодневных нет (кроме 1,5 дня). На zillertal.at это flexipass Superskipass, то есть по всей долине. Точнее писать `4-in-6 flexipass (Zillertal Superskipass): €317.50` / ES `Flexipass 4 en 6 (Zillertal Superskipass): 317,50 €`. Сравнение с 4 × €82 остаётся корректным: flexipass дешевле и покрывает больше |
| 36 | 4 × €82 = €328 против €317,50, экономия €10,50 (L250, L267, L297) | арифметика | 2026-10-30 | верно | — |
| 37 | Голос: «Same ski area. Four ticket prices.» (L258) | п. 24–27: четыре цены дневного билета по времени начала (1,5 дня не в счёт) | 2026-10-30 | верно | — Необязательно: билеты с 10:30, 12:00 и 13:30 продаются только в кассе, онлайн есть только билет с 8:00. Группе со смешанным планом это пригодится, можно добавить в подпись |

## Утверждения о продукте

Сверено с обновлённым `CLAUDE.md`, строки 21–33.

| # | Утверждение | Вердикт | Что заменить |
|---|---|---|---|
| 38 | Подпись v3 L276 / L306: «Plan the rest of the trip day by day, with a map and real places, in PlanVIA», то есть PlanVIA строит маршрут по Zell am Ziller. То же для Вены и Нюрнберга в v1 L74 / L104 и для Вены в v2 L175 / L205 | **не подтвердилось** | В продукте AI-маршрут есть «для 100+ направлений», но списка нет ни в `CLAUDE.md`, ни на goplanvia.com (главная говорит только «real places for 100+ destinations»), а `plan/questions.md` ответа не содержит. В v3 это ещё и противоречит собственной оговорке автора L252 «Что НЕ утверждаем: что PlanVIA умеет строить план именно для Цилерталя». **Условие для Ярослава при одобрении:** подтвердить Вену, Нюрнберг и Zell am Ziller (открытый вопрос 2 черновика). Если какого-то направления нет, заменить в соответствующей подписи EN: «Pick the dates together in PlanVIA, the AI group trip planner: invite your friends, vote, chat with your group and share the plan. Create a trip: goplanvia.com (link in bio).» ES: «Elegid las fechas juntos en PlanVIA, el planificador de viajes en grupo con IA: invitad a vuestros amigos, votad, hablad en el chat del grupo y compartid el plan. Crea un viaje: goplanvia.com (enlace en la bio).» Все глаголы здесь разрешены `CLAUDE.md` L33 |
| 39 | ES-фраза о продукте в описании Shorts (L110, L211, L312) и «el planificador de viajes en grupo con IA» | не подтвердилось | Дословно совпадает с `CLAUDE.md`, но там помечена «черновик, ждёт утверждения Ярослава» (вопрос 10). Утверждает Ярослав в том же пакете |
| 40 | Финальные карточки и подписи: «Create a trip», «Day-by-day plan · map · real places · share the plan», «copy a ready plan» | верно | Всё это есть в продукте (`CLAUDE.md` L25–27). Рекомендация: в `CLAUDE.md` для ссылок указан только один готовый план, Португалия. Готового плана по Вене, Нюрнбергу или Циллерталю зритель не найдёт, поэтому в v1 L74 и v3 L276 лучше оставить только «Create a trip» |

Запрещённого нет: «split the budget», «track who owes what», «split», «owes» и личного кошелька билетов в тексте нет. Фраза «budgets can differ» / «caben presupuestos distintos» (L165, L195) о групповой динамике, это не обещание функции. Аудитория только Европа: данных по рынку США и аргументов для американской аудитории в сценариях нет.

Новое в продукте можно использовать, но это не обязательно. В v1 хук про выбор выходных («let's decide closer to the date»), а в v2 пузыри группового чата. Туда естественно ложатся «vote on the weekend» и «chat with your group». Решать автору и Ярославу, на фактчек это не влияет.

## Стоп-слова и бренд

- Стоп-слова (hidden gem, nestled, bucket list, breathtaking, vibrant, must-see, unforgettable, embark, delve, «whether you're… or…», «fast-paced») и «sign up» не найдены.
- Бренд: везде **PlanVIA**. Planvia, PlanVia, planvia вне домена и yourplanvia.com не встречаются. Домен goplanvia.com.
- Первое упоминание с категорией есть: в голосе («Plan it in PlanVIA, the AI group trip planner»), в подписях и на финальной карточке («PlanVIA: AI Group Trip Planner»). EN-фраза о продукте в описании Shorts дословно совпадает с `CLAUDE.md`.
- Метка AI-контента стоит во всех трёх роликах: «AI-generated visuals» в последних 2 с, «Visuals are AI-generated» / «Imágenes generadas con IA» в подписи, плюс встроенная метка платформ при загрузке. Открыт вопрос 4: умеет ли Postiz ставить флаг через API. Если не умеет, флаг вручную ставит Ярослав при публикации, иначе ролик без флага не выпускать.
- Промпты fal.ai: людей, силуэтов, рук и знаменитостей нет. Суффикс «No people, no crowds, no silhouettes, no hands, no text, no numbers, no logos, no brand names» применяется ко всем трём наборам (L115, L215, L316). Логотипы отдельно исключены: кружки без принтов (mkt-04), лыжи без марок (ski-03), кабинки без надписей (ski-04), интерфейс PlanVIA не рисуется. Кадры mkt-02 и nye-05 (неоготическая ратуша с катком) и mkt-03 (готический фонтан) похожи на реальные места Вены и Нюрнберга. Правила `CLAUDE.md` это не запрещают, но поэтому AI-метка на них обязательна, и автор её ставит.

## Строки `data/place-facts.csv` от social-producer (124–140)

| Строка | Что | Вердикт |
|---|---|---|
| 124 | Нюрнберг: даты, церемония 27.11 в 17:30 | верно |
| 125 | Нюрнберг: часы, день открытия, пауза, 24.12 | верно |
| 126 | до 180 палаток; более 2 млн посетителей в 2025 | верно (Ausblick: «mehr als zwei Millionen Besucherinnen und Besucher») |
| 127 | Нюрнберг: цены не опубликованы | на портале при проверке цен не встретил; отдельно не искал. В роликах не используется |
| 128 | Вена: даты, часы, 24.12, 44 дня | данные верны. Но DE-ссылка из заметок у меня открылась как EN-страница, поэтому немецкие цитаты «Täglich 10-22 Uhr» и др. не подтверждены. Уточнение — новая строка A ниже |
| 129 | Вена: цены не опубликованы | верно |
| 130 | Каток: 13.11.2026 – 06.01.2027, 10–22, 24.12 до 18:30, 31.12 закрыт | верно по EN; «31.12. geschlossen» на DE не подтверждено (см. строку A) |
| 131 | Silvesterpfad: дата, часы, вход, еда с 11:00 | верно; «в карточках пять» — уточнение в строке B |
| 132 | Pummerin, «Голубой Дунай», запрет F2 | верно |
| 133 | Концерт 1.1.2027 с 11:15, Stephansplatz и Riesenradplatz; бесплатность не заявлена | верно |
| 134 | Гала-ужины: цены не опубликованы | не проверял, в роликах не используется |
| 135 | Цены дневных билетов, 1,5 дня €121,50, «cash desk only» кроме 8:00 | верно (сноска WebFetch «[проверить вручную]» про кассу подтверждена). Цены PDF 2025/26 не проверял, они не используются |
| 136 | 4 in 6 €317,50; 5 in 7 €391; 6 in 7 €429,50; 10 in 14 €715; обмен, продление, перенос невозможны | цены верны; по условиям AGB: «Subsequent exchange for another ski pass, transfer to another person, extension or postponement…», «The ski passes and day tickets are not transferable!». К какому продукту относится, уточняет строка C |
| 137 | Сезоны Арены, Gerlosstein, Superskipass | верно |
| 138 | Групповые условия, нет скидок студентам и пенсионерам, залог за карту €2 | верно: «No student or senior citizen discounts are offered in the entire Zillertal», «A deposit fee of € 2,00 is due for the chip card, which will be reimbursed» |
| 139 | Групповая арифметика | верно |
| 140 | Полные выходные: 6 и 4 | верно |

### Новые строки для `data/place-facts.csv` (checked_by=fact-checker)

Ошибочных цифр нет. Нашёл три неточности в источниках и атрибуции, ниже готовые строки. **В CSV сам не дописал:** у меня есть только полная перезапись файла (Write), без Edit и дозаписи, а перезаписывать 140 строк чужих данных в каталоге без git рискованно. Координатору: добавить три строки в конец файла как есть.

```csv
Wien,Wiener Christkindlmarkt am Rathausplatz 2026,source_recheck,"13 Nov – 26 Dec 2026; daily 10:00–22:00; 24 Dec 10:00–18:30; 44 operating days; Vienna Ice World 13 Nov 2026 – 6 Jan 2027, 31 Dec closed",,https://www.wien.info/en/now-on/christmas/christmas-markets-342664,2026-10-30,fact-checker,"Данные строк social-producer (Wien) подтверждены. Ссылку давать без ?pp=1. DE-ссылка https://www.wien.info/de/jetzt-aktuell/weihnachten/weihnachtsmaerkte-342664 при проверке открылась как эта EN-страница, поэтому немецкие цитаты («Täglich 10-22 Uhr», «31.12. geschlossen») не подтверждены, данные совпадают. PDF christkindlmarkt.at — Ausschreibung для участников (Bewerbungsfrist 19.01–19.03.2026): «Marktzeitraum: 13.11.2026 – 26.12.2026 (entspricht 44 Betriebstage)», «24.12.2026: 10:00 – 18:30 Uhr»"
Wien,Silvesterpfad 2026/27,locations_and_canonical_url,"page says 'eight locations' but gives no list of eight: route Freyung – Am Hof – Graben – Stephansplatz – Kärntner Straße – Neuer Markt, plus Rathausplatz and Prater/Riesenradplatz",,https://www.wien.info/en/now-on/christmas/new-years-eve-354224,2026-10-30,fact-checker,"Уточнение к строке social-producer «в карточках пять»: названо больше пяти мест, что считать «локацией», страница не уточняет — число не использовать. Дата, 14:00–02:00, бесплатный вход, еда с 11:00, Pummerin, запрет F2, концерт 1.1.2027 с 11:15 подтверждены на EN и DE. Каноничный DE-URL: https://www.wien.info/de/aktuell/weihnachten/silvester-358870 (ссылка /de/musik-buehne/silvester-358870 перенаправляет туда)"
Zell am Ziller (Tirol),Zillertaler Superskipass,flexipass_2026_27,"flexipass 4 in 6 317.50; 5 in 7 391.00; 6 in 7 429.50; 10 in 14 715.00 (adult), listed under Zillertaler Superskipass tariffs 2026/2027",EUR,https://www.zillertal.at/en/winter/holidays/zillertal-superskipass.html,2026-10-30,fact-checker,"Уточнение к строке social-producer elective_tickets_2026_27 (Zillertal Arena). На zillertalarena.com/en/winter/ski-area/tickets-prices/ эти билеты идут разделом «Elective tickets» после Zillertaler Superskipass, без указания зоны; многодневных билетов только для Арены нет (кроме 1,5 дня), Superskipass «from 2 days valid throughout Zillertal & Wildkogel-Bramberg». На zillertal.at это flexipass Superskipass. Сезон на странице zillertal.at подписан непоследовательно («Tarifs 2026/2027» и «winter season 2025/2026»), цены совпадают с zillertalarena.com 2026–27. Писать «4-in-6 flexipass (Zillertal Superskipass)», а не «Zillertal Arena 4-in-6»"
```

## Что нужно до публикации

1. **v1:** можно нести Ярославу сейчас. При одобрении он отвечает на вопрос 2 (Вена, Нюрнберг); если какого-то направления нет, подставить замену из п. 38.
2. **v2:** автор правит 70/30 (п. 21) в EN и ES: титр, голос и подпись. После этого нести Ярославу, факты повторно проверять не нужно.
3. **v3:** можно нести Ярославу. При одобрении — вопрос 2 (Zell am Ziller) и замена из п. 38, если направления нет. Рекомендации п. 33 и 35 по желанию. Цены перепроверить накануне публикации 9–13 нояб.
4. **Для всех трёх:** если Postiz не ставит флаг AI-контента, его ставит Ярослав вручную при загрузке (вопрос 4).
5. **Координатору:** дописать три строки выше в `data/place-facts.csv`.
