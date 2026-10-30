# Зимние ролики: 3 сценария, EN + ES (30.10.2026)

Задача: backlog W3-02 / W3-03. Исполнитель: social-producer.
Статус: сценарии готовы, ждут фактчекера, затем одобрения Ярослава пакетом. Медиа НЕ генерировались (n8n с fal.ai не подключён), в Postiz ничего не ставилось. Есть только промпты.

Формат всех трёх: вертикальный 9:16 (1080×1920), 36 секунд, TikTok / Reels / Shorts, один монтаж на обе платформы. Кадры fal.ai без текста и без людей: один набор кадров на EN и ES, различаются только титры и озвучка.

Дата проверки всех фактов: 30.10.2026. Новые строки добавлены в `data/place-facts.csv` (checked_by=social-producer).

| ID | Тема | Города / места | Окно публикации (предложение) |
|---|---|---|---|
| v1-christmas-markets | Рождественские ярмарки с друзьями: выбрать выходные | Вена (Rathausplatz), Нюрнберг | 2–6 нояб. Вена открывается 13 нояб., после этой даты хук теряет смысл |
| v3-ski-zillertal | Лыжи с друзьями: цена ски-пасса, групповая арифметика | Zillertal Arena (Zell am Ziller, Тироль) | 9–13 нояб. Сезон открывается 4 дек. |
| v2-nye-vienna | Новый год с друзьями: кто бронирует, разные бюджеты | Вена | 16–27 нояб. |

Публикация по правилам из `plan/specs/n8n-social-flow.md`: EN утром, ES вечером, одни и те же аккаунты.

## Общие правила для всех роликов

- Озвучка: спокойный дружелюбный тон, без «рекламного» напора. Кто озвучивает (голос Ярослава, TTS или только титры) — открытый вопрос 1 ниже. Дикция EN ~2,4 слова/с; ES в тех же окнах плотнее (~2,8 слова/с), при записи допустимо +1–2 с, итог не больше 40 с. Фраза в хуке — 5–6 слов, допустимо до 2,5 с; текст хука на экране появляется в первые 1,5 с.
- Титры вжигаем на языке версии, безопасная зона: без текста в нижних 20% и правых 15% кадра (интерфейс платформ).
- На каждом ролике в последних 2 с мелким шрифтом: `Checked 30 Oct 2026 · <источники> · AI-generated visuals` (ES: `Revisado: 30 oct 2026 · … · Imágenes generadas con IA`).
- Метка AI-контента: да, на всех трёх. Включаем встроенную метку TikTok / Instagram / YouTube при загрузке. Умеет ли Postiz ставить этот флаг через API — не проверено, вопрос 4.
- Кадры fal.ai показывают «типичную» ярмарку, площадь, склон, а не съёмку реального места. Поэтому метка AI обязательна, а в подписи нет слов «вот как выглядит». Если Ярослав захочет точные виды — заменить на собственные или лицензионные фото.
- Интерфейс PlanVIA fal.ai не рисуем (фейковый UI вводит в заблуждение). В финале либо запись экрана настоящего продукта (нужен материал, вопрос 14 в `plan/questions.md`), либо текстовая карточка на фоне из fal.ai (кадр `*-07`). Сценарии написаны так, что работают с любой из двух.
- Что показываем о продукте (всё есть сейчас): AI-маршрут по дням, карта, реальные места, каталог готовых планов («copy a ready plan»), «share the plan». Не использованы формулировки, которых в продукте нет (запрещённые слова из CLAUDE.md).
- Музыка: из библиотеки платформы или с лицензией без ограничений; без узнаваемых треков.
- Групповая арифметика («6 друзей») — пример, а не статистика; в подписи помечена как «our math» / «nuestra cuenta».

---

## v1-christmas-markets

```markdown
# Ролик: Christmas market with friends — pick the weekend first
- Платформы: TikTok, Reels, Shorts
- Язык: EN / ES
- Источник цифр: таблица ниже, строки в data/place-facts.csv (Nürnberg, Wien, 30.10.2026)
```

### Факты

| В ролике | Значение | Источник | Статус |
|---|---|---|---|
| Вена, Rathausplatz: даты и часы | 13 нояб. – 26 дек. 2026; ежедневно 10:00–22:00; 24 дек. 10:00–18:30 | https://www.wien.info/en/now-on/christmas/christmas-markets-342664?pp=1 (то же на DE-странице wien.info и в документе организатора https://www.christkindlmarkt.at/wp-content/uploads/2026/01/01_Wiener-Christkindlmarkt-2026_Information-Standbewerbung.pdf: «44 Betriebstage») | официальный, 30.10.2026 |
| Нюрнберг: старт | пятница 27 нояб. 2026 (церемония 17:30); работает до 24 дек. | https://www.nuernberg.de/internet/kommunikation_stadtmarketing_en/christmas_market.html, https://www.nuernberg.de/imperia/md/kommunikation_stadtmarketing/dokumente/internet/ckm/ckm_26_information_en.pdf | официальный, 30.10.2026 |
| Нюрнберг: часы | ежедневно 10:00–21:00 (в день открытия до 22:00); 24 дек. 10:00–14:00 | https://www.nuernberg.de/internet/stadtportal/christkindlesmarkt.html | официальный, 30.10.2026 |
| Нюрнберг: размер | до 180 палаток («bis zu 180 Buden») | https://www.nuernberg.de/imperia/md/kommunikation_stadtmarketing/dokumente/internet/ckm/ckm_26_ausblick.pdf | официальный, 30.10.2026 |
| Полные выходные (сб+вс) внутри дат | Вена 6 (14–15, 21–22, 28–29 нояб.; 5–6, 12–13, 19–20 дек.); Нюрнберг 4 (28–29 нояб.; 5–6, 12–13, 19–20 дек.) | расчёт по календарю 2026 от дат выше | расчёт автора, проверен |
| Цены: вход, залог за кружку, глинтвейн | В ролике НЕТ | на официальных страницах не указаны | `[проверить вручную]`, если понадобятся |

### EN

#### Хук (0–2 с)
Текст на экране: `Christmas market with friends? 2 dates.` и мелко пузырь чата (без брендинга мессенджеров): `"let's decide closer to the date"`
Голос: «Christmas market with friends? Two dates.»

#### Раскадровка

| Время | Кадр | Текст на экране | Озвучка |
|---|---|---|---|
| 2–9 с | mkt-02 (Вена) | `VIENNA · Rathausplatz`<br>`13 Nov – 26 Dec`<br>`daily 10:00–22:00` | «Vienna's Rathausplatz market: November 13 to December 26, open daily, ten to ten.» |
| 9–16 с | mkt-03 (Нюрнберг), вставка mkt-04 на последние 2 с | `NUREMBERG`<br>`opens Fri 27 Nov`<br>`daily 10:00–21:00 · up to 180 stalls` | «Nuremberg opens Friday, November 27: up to 180 stalls, open ten to nine every day.» |
| 16–23 с | mkt-05 | `Full weekends inside the dates`<br>`Vienna 6 · Nuremberg 4` | «Count the weekends: Vienna six, Nuremberg four. With a group, the date is the hard part.» |
| 23–29 с | mkt-06 | `24 Dec`<br>`Nuremberg closes 14:00`<br>`Vienna closes 18:30` | «Arriving on the 24th? Nuremberg closes at two p.m., Vienna at six thirty.» |
| 29–36 с | mkt-07 или запись экрана | `Create a trip: goplanvia.com`<br>`PlanVIA: AI Group Trip Planner`<br>`Day-by-day plan · map · real places · share the plan` | «Plan it in PlanVIA, the AI group trip planner. Share the plan. Link in bio.» |

Финал: «Plan it in PlanVIA, the AI group trip planner. Share the plan. Link in bio.»

#### Подпись

```
Christmas market with friends? Vienna's Rathausplatz market runs 13 Nov to 26 Dec (daily 10:00-22:00). Nuremberg's opens Fri 27 Nov and closes 24 Dec at 14:00. Count the full weekends inside those dates: 6 in Vienna, 4 in Nuremberg.
Plan it day by day, with a map and real places, in PlanVIA, the AI group trip planner. Create a trip or copy a ready plan: goplanvia.com (link in bio).
Sources: wien.info, nuernberg.de. Checked 30 Oct 2026. Visuals are AI-generated.
#ChristmasMarkets #GroupTravel #TripWithFriends #Vienna #Nuremberg
```

Shorts, заголовок: `Christmas markets with friends: Vienna vs Nuremberg dates`
Shorts, описание (в начало подписи): `PlanVIA is an AI group trip planner: plan a trip with friends in minutes, with a day-by-day itinerary, a map and real places.`

### ES

#### Хук (0–2 с)
Текст на экране: `¿Mercado navideño con amigos? 2 fechas.` и мелко пузырь чата: `"lo decidimos más cerca de la fecha"`
Голос: «¿Mercado navideño con amigos? Dos fechas.»

#### Раскадровка

| Время | Кадр | Текст на экране | Озвучка |
|---|---|---|---|
| 2–9 с | mkt-02 | `VIENA · Rathausplatz`<br>`13 nov – 26 dic`<br>`todos los días 10:00–22:00` | «Viena, Rathausplatz: del 13 de noviembre al 26 de diciembre, de 10 a 22 h.» |
| 9–16 с | mkt-03, вставка mkt-04 | `NÚREMBERG`<br>`abre el vie 27 nov`<br>`todos los días 10:00–21:00 · hasta 180 puestos` | «Núremberg abre el viernes 27 de noviembre: hasta 180 puestos, de 10 a 21 h todos los días.» |
| 16–23 с | mkt-05 | `Fines de semana completos`<br>`Viena 6 · Núremberg 4` | «Contad los fines de semana: Viena, seis; Núremberg, cuatro. En grupo, lo difícil es la fecha.» |
| 23–29 с | mkt-06 | `24 dic`<br>`Núremberg cierra a las 14:00`<br>`Viena cierra a las 18:30` | «¿Llegáis el 24? Núremberg cierra a las 14:00; Viena, a las 18:30.» |
| 29–36 с | mkt-07 или запись экрана | `Crea un viaje: goplanvia.com`<br>`PlanVIA: AI Group Trip Planner`<br>`Plan día a día · mapa · lugares reales · comparte el plan` | «Organizadlo en PlanVIA, el planificador de viajes en grupo con IA. Compartid el plan. Enlace en la bio.» |

Финал: «Organizadlo en PlanVIA, el planificador de viajes en grupo con IA. Compartid el plan. Enlace en la bio.»

#### Подпись

```
¿Mercado navideño con amigos? El de la Rathausplatz de Viena va del 13 de nov al 26 de dic (todos los días, 10:00-22:00). El de Núremberg abre el vie 27 de nov y cierra el 24 de dic a las 14:00. Contad los fines de semana completos dentro de esas fechas: 6 en Viena, 4 en Núremberg.
Planificadlo día a día, con mapa y lugares reales, en PlanVIA, el planificador de viajes en grupo con IA. Crea un viaje o copia un plan listo: goplanvia.com (enlace en la bio).
Fuentes: wien.info, nuernberg.de. Revisado: 30 oct 2026. Imágenes generadas con IA.
#MercadosNavideños #ViajesEnGrupo #ViajarConAmigos #Viena #Núremberg
```

Shorts, заголовок: `Mercados navideños con amigos: fechas de Viena y Núremberg`
Shorts, описание: `PlanVIA es un planificador de viajes en grupo con IA: organiza un viaje con amigos en minutos, con un itinerario día a día, un mapa y lugares reales.` (ES-фраза — черновик, ждёт утверждения Ярослава, вопрос 10)

### Медиа (fal.ai, общие для EN и ES)

Пометка AI-контента: да.
К каждому промпту добавлять: `Photorealistic, vertical 9:16, cinematic soft lighting. No people, no crowds, no silhouettes, no hands, no text, no numbers, no logos, no brand names.` Движение — image-to-video, клип до 5 с; на длинные окна растягиваем замедлением 0,7× и медленным зумом в монтаже.

| Кадр | Окно | Промпт (картинка) | Движение |
|---|---|---|---|
| mkt-01 | 0–2 с | Empty Christmas market square at blue hour, rows of wooden stalls with red-and-white striped cloth roofs, warm string lights, light snowfall, a lit gothic church tower in the background, wet cobblestones reflecting the lights. | Slow push-in along the stall row, snowflakes drifting, lights twinkle softly. |
| mkt-02 | 2–9 с | Neo-Gothic city hall with a tall central spire lit warm gold at dusk, a wide square in front filled with wooden market huts and decorated fir trees, a softly glowing ice rink on one side, bare trees with white lights. | Slow tilt up from the huts to the spire, gentle haze. |
| mkt-03 | 9–16 с | Narrow lanes of stalls with red-and-white striped cloth roofs on a medieval German market square, gingerbread, nuts and wooden toys on the counters, an ornate gothic stone fountain spire in the background, warm lamp light, frosty evening. | Slow sideways glide along the stall counters. |
| mkt-04 | вставка 2 с | Close-up of two plain ceramic mugs of steaming mulled wine on a wooden stall counter, blurred market lights behind, mugs without any print. | Steam rising, slow focus pull. |
| mkt-05 | 16–23 с | Top-down flat lay on dark wood: an advent calendar with small plain unnumbered doors, pine twigs, cinnamon sticks, star anise, two small candles, warm light, empty space in the center. | Slow top-down zoom, candle flames flicker. |
| mkt-06 | 23–29 с | Quiet market lane at dusk with stall shutters half closed, dimmed string lights, a single paper star lantern glowing, thin snow on the roofs. | Lights slowly dim, snow falls. |
| mkt-07 | 29–36 с | Soft dark-green gradient background with slowly falling snowflake particles and faint warm bokeh of Christmas lights at the bottom, large empty space in the center for text. | Snow particles drift. |

---

## v2-nye-vienna

```markdown
# Ролик: New Year's Eve in Vienna with friends — the entry is free, the group chat is not
- Платформы: TikTok, Reels, Shorts
- Язык: EN / ES
- Источник цифр: таблица ниже, строки в data/place-facts.csv (Wien, 30.10.2026)
```

Без выдуманных цифр: все числа в ролике — даты и часы с официальной страницы wien.info. Про деньги и «кто платит» — только групповая динамика словами, без сумм. Вена выбрана потому, что программа 2026/27 уже опубликована на официальном портале; у Мадрида, Лиссабона и Эдинбурга она пока не вышла или не найдена на первоисточнике.

### Факты

| В ролике | Значение | Источник | Статус |
|---|---|---|---|
| Silvesterpfad | 31 дек. 2026, 14:00–02:00; вход свободный; еда и напитки с 11:00 | https://www.wien.info/en/now-on/christmas/new-years-eve-354224 (DE: https://www.wien.info/de/musik-buehne/silvester-358870) | официальный, 30.10.2026 |
| Полночь | звонит колокол Pummerin в соборе св. Стефана, танцуют «Голубой Дунай» | та же страница | официальный, 30.10.2026 |
| Пиротехника | ракеты и петарды (от категории F2) запрещены во всей Вене | та же страница | официальный, 30.10.2026 |
| Каток у Ратуши | 31 дек. закрыт (сезон 13 нояб. 2026 – 6 янв. 2027) | https://www.wien.info/en/now-on/christmas/christmas-markets-342664?pp=1 («Vienna Ice World»: «Dec 31: closed»; на DE-странице «31.12. geschlossen») | официальный, 30.10.2026 |
| Новогодний концерт | 1 янв. 2027, трансляция из Musikverein с 11:15 на экранах на Stephansplatz и Riesenradplatz | страница Silvester | официальный, 30.10.2026, только в титрах и подписи |
| Правило 70/30 | именованное правило PlanVIA, как в постах LinkedIn от 30.10 | `content/social/2026-10-30-linkedin-posts.md` | в ролике применено к ночи: ужин и полночь вместе (70%), остальное по желанию (30%); правка по фактчеку 30.10 |

Не используем: число локаций Silvesterpfad. Страница пишет «eight locations», но в карточках пять (Stephansplatz, Graben, Freyung, Rathausplatz, Prater). Цены и билеты галa-ужинов на wien.info не указаны, в ролике их нет. Данные страницы wien.gv.at «Vienna New Year's Eve Trail 2025/2026» относятся к прошлому сезону и не использовались.

### EN

#### Хук (0–2 с)
Текст на экране: `Vienna, 31 Dec: street party, free entry`
Голос: «Vienna, New Year's Eve: free entry.»

#### Раскадровка

| Время | Кадр | Текст на экране | Озвучка |
|---|---|---|---|
| 2–9 с | nye-02 | `SILVESTERPFAD`<br>`31 Dec 2026 · 14:00–02:00`<br>`free admission` | «The Silvesterpfad runs from 2 p.m. to 2 a.m. on December 31. Free admission.» |
| 9–16 с | nye-03 | пузыри чата (без брендинга мессенджеров):<br>`"who's booking the apartment?"`<br>`"who pays first?"`<br>`"still checking prices"` | «The hard part is the group chat: who books, who pays first, who's still "checking prices".» |
| 16–23 с | nye-04, на последние 2 с вставка nye-06 | `70/30`<br>`70% together: dinner + midnight · 30% your call`<br>мелко: `1 Jan, 11:15: New Year's Concert on big screens at Stephansplatz` | «Our 70/30 rule: dinner and midnight together, the rest of the night is your call. Entry is free, so budgets can differ.» |
| 23–30 с | nye-05 | `Tell the group:`<br>`Ice rink at the Rathaus: closed 31 Dec`<br>`Rockets and firecrackers (F2+): banned in all of Vienna` | «Tell the group: the rink is closed on the 31st, and rockets and firecrackers (F2 up) are banned citywide.» |
| 30–36 с | nye-07 или запись экрана | `Create a trip: goplanvia.com`<br>`PlanVIA: AI Group Trip Planner`<br>`Day-by-day plan · map · real places · share the plan` | «Put it all in one plan: PlanVIA, the AI group trip planner. Link in bio.» |

Финал: «Put it all in one plan: PlanVIA, the AI group trip planner. Link in bio.»

#### Подпись

```
New Year's Eve in Vienna with friends: the Silvesterpfad street party runs 31 Dec, 14:00-02:00, with free admission. At midnight the Pummerin bell rings at St. Stephen's Cathedral and the Blue Danube plays. Keep the shared part simple (our 70/30 rule: dinner and midnight together, the rest of the night is your call) and agree who books the apartment before you pick the restaurant. Heads-up: the ice rink at the Rathaus is closed on 31 Dec, and rockets and firecrackers (category F2 and up) are banned in all of Vienna. 1 Jan: New Year's Concert on big screens from 11:15.
Put the plan in one place: PlanVIA, the AI group trip planner, with a day-by-day itinerary, a map and real places. Create a trip: goplanvia.com (link in bio).
Source: wien.info. Checked 30 Oct 2026. Visuals are AI-generated.
#NewYearsEve #Vienna #GroupTravel #TripWithFriends #Silvester
```

Shorts, заголовок: `New Year's Eve in Vienna with friends: what's free, what to agree`
Shorts, описание: `PlanVIA is an AI group trip planner: plan a trip with friends in minutes, with a day-by-day itinerary, a map and real places.`

### ES

#### Хук (0–2 с)
Текст на экране: `Viena, 31 dic: fiesta en la calle, entrada gratis`
Голос: «Nochevieja en Viena: entrada gratis.»

#### Раскадровка

| Время | Кадр | Текст на экране | Озвучка |
|---|---|---|---|
| 2–9 с | nye-02 | `SILVESTERPFAD`<br>`31 dic 2026 · 14:00–02:00`<br>`entrada gratuita` | «El Silvesterpfad se celebra el 31 de diciembre, de 14:00 a 2:00. Entrada gratuita.» |
| 9–16 с | nye-03 | пузыри чата:<br>`"¿quién reserva el piso?"`<br>`"¿quién paga primero?"`<br>`"sigo mirando precios"` | «Lo difícil es el chat del grupo: quién reserva, quién paga primero, quién sigue "mirando precios".» |
| 16–23 с | nye-04, вставка nye-06 | `70/30`<br>`70% juntos: cena + medianoche · 30%, a tu aire`<br>мелко: `1 ene, 11:15: Concierto de Año Nuevo en pantallas en Stephansplatz` | «Regla 70/30: cena y medianoche juntos; el resto de la noche, a vuestro aire. Con entrada gratis, caben presupuestos distintos.» |
| 23–30 с | nye-05 | `Avisad al grupo:`<br>`Pista de hielo del Rathaus: cerrada el 31 dic`<br>`Cohetes y petardos (F2 o más): prohibidos en toda Viena` | «Avisad: la pista de hielo cierra el 31 y los cohetes (F2 o más) están prohibidos en toda la ciudad.» |
| 30–36 с | nye-07 или запись экрана | `Crea un viaje: goplanvia.com`<br>`PlanVIA: AI Group Trip Planner`<br>`Plan día a día · mapa · lugares reales · comparte el plan` | «Todo en un plan: PlanVIA, el planificador de viajes en grupo con IA. Enlace en la bio.» |

Финал: «Todo en un plan: PlanVIA, el planificador de viajes en grupo con IA. Enlace en la bio.»

#### Подпись

```
Nochevieja en Viena con amigos: el Silvesterpfad, la fiesta callejera, es el 31 de dic de 14:00 a 2:00 y la entrada es gratuita. A medianoche suena la campana Pummerin en la catedral de San Esteban y se baila el Danubio azul. Mantened sencilla la parte común (nuestra regla 70/30: cena y medianoche juntos; el resto de la noche, a vuestro aire) y decidid quién reserva el piso antes de elegir restaurante. Ojo: la pista de hielo del Rathaus cierra el 31 de dic, y los cohetes y petardos (categoría F2 o superior) están prohibidos en toda Viena. El 1 de ene: Concierto de Año Nuevo en pantallas grandes desde las 11:15.
Todo en un plan: PlanVIA, el planificador de viajes en grupo con IA, con itinerario día a día, mapa y lugares reales. Crea un viaje: goplanvia.com (enlace en la bio).
Fuente: wien.info. Revisado: 30 oct 2026. Imágenes generadas con IA.
#Nochevieja #Viena #ViajesEnGrupo #ViajarConAmigos #FinDeAño
```

Shorts, заголовок: `Nochevieja en Viena con amigos: qué es gratis y qué acordar`
Shorts, описание: `PlanVIA es un planificador de viajes en grupo con IA: organiza un viaje con amigos en minutos, con un itinerario día a día, un mapa y lugares reales.` (черновик, вопрос 10)

### Медиа (fal.ai, общие для EN и ES)

Пометка AI-контента: да. Суффикс и правила движения те же, что в v1. Пузыри чата рисуем титрами, не fal.ai.

| Кадр | Окно | Промпт (картинка) | Движение |
|---|---|---|---|
| nye-01 | 0–2 с | Winter night in a historic European city center: a wide pedestrian street leading to a lit gothic cathedral spire, streamers and confetti on the wet pavement, warm street lamps, bokeh lights. | Slow push-in, confetti flutters. |
| nye-02 | 2–9 с | Empty open-air festival stage on a historic square at dusk, a large dark LED screen switched off, warm string lights across the square, wooden barriers, a food stall with steaming pots, frost in the air. | Slow lateral glide, string lights switch on one after another. |
| nye-03 | 9–16 с | Cozy city apartment living room at night: a long dining table set for dinner with candles, glasses and plates, string lights, a big window showing a snowy rooftop skyline with a distant cathedral spire. | Candle flames flicker, slow push-in toward the window. |
| nye-04 | 16–21 с | Close-up of an analog wall clock with simple tick marks and no numerals, both hands at 12 o'clock, soft golden bokeh lights behind. | Second hand ticks, golden light pulses. |
| nye-05 | 23–30 с | Empty outdoor ice rink at night in front of a lit neo-Gothic town hall, rink lit blue-white, a plain barrier chain across the entrance gap, bare trees with string lights. | Slow pan across the rink, chain sways. |
| nye-06 | вставка 2 с (21–23 с) | Quiet cobblestone street at sunrise on New Year's morning, pale pink sky, a few scattered confetti pieces, a cafe table with two coffee cups and a croissant. | Sunlight creeps across the street. |
| nye-07 | 30–36 с | Deep midnight-blue gradient background with slowly rising golden bokeh sparks, large empty space in the center for text. | Sparks rise slowly. |

---

## v3-ski-zillertal

```markdown
# Ролик: Ski day with friends — one lift, four prices
- Платформы: TikTok, Reels, Shorts
- Язык: EN / ES
- Источник цифр: таблица ниже, строки в data/place-facts.csv (Zell am Ziller, 30.10.2026)
```

### Факты

| В ролике | Значение | Источник | Статус |
|---|---|---|---|
| Взрослый дневной ски-пасс Zillertal Arena, зима 2026/27 | с 8:00/8:30/9:00 — €82,00; с 10:30 — €78,50; с 12:00 — €63,50; с 13:30 — €45,00 | https://www.zillertalarena.com/en/zell/winter/ski-pass-prices/ (заголовок «Zillertal Arena Ski Pass Prices 2026–27») | официальный, 30.10.2026 |
| Билет «4 in 6» | €317,50 за 4 дня катания на выбор в пределах 6 дней | https://www.zillertalarena.com/en/winter/ski-area/tickets-prices/ | официальный, 30.10.2026 |
| Сезон | 4 дек. 2026 – 11 апр. 2027, «with sufficient snow» | та же страница | официальный, 30.10.2026 |
| Групповая скидка | 10% от 11 человек, 15% от 35 (билеты на 1 и 1,5 дня, покупает один человек) | https://www.zillertalarena.com/en/winter/ski-area/tickets-prices/group-offer/, https://www.zillertalarena.com/fileadmin/userdaten/docs/01-arena/Gruppenangebot_Winter_2026_2027_ENG.pdf | официальный, 30.10.2026 |
| Оговорка | «Prices may be subject to change» | страница цен | вынесена в подпись |
| 6 × €82 | €492 | арифметика | проверено |
| 2 в 8:00 + 2 в 10:30 + 2 в 13:30 | 164 + 157 + 90 = €411 (разница с €492: €81) | арифметика от цен выше | проверено |
| Присоединился после обеда | 82 − 45 = €37 | арифметика | проверено |
| 4 × €82 против «4 in 6» | €328 против €317,50: экономия €10,50 | арифметика | проверено; в ролике честно «небольшая экономия, смысл в гибкости» |

Что НЕ утверждаем: что PlanVIA умеет строить план именно для Цилерталя (открытый вопрос 2), что поздний пасс «такой же по катанию» (на экране и в подписи сказано, что катаешься меньше).

### EN

#### Хук (0–2 с)
Текст на экране: `6 friends, 1 ski day: 4 prices`
Голос: «Same ski area. Four ticket prices.»

#### Раскадровка

| Время | Кадр | Текст на экране | Озвучка |
|---|---|---|---|
| 2–9 с | ski-02 | `ZILLERTAL ARENA · adult day ticket · winter 2026/27`<br>`from 8:00  €82`<br>`from 10:30  €78.50`<br>`from 12:00  €63.50`<br>`from 13:30  €45`<br>мелко: `season 4 Dec – 11 Apr, snow permitting` | «Zillertal Arena adult day ticket, winter 2026/27: 82 euros from eight a.m., 45 from one-thirty.» |
| 9–16 с | ski-03, на последние 2 с вставка ski-05 | `6 × €82 = €492` (все в 8:00)<br>`2 at 8:00 + 2 at 10:30 + 2 at 13:30 = €411`<br>`Joins after lunch? −€37 (and skis less)` | «Six friends on the 8 a.m. ticket: 492 euros. Two early, two mid-morning, two after lunch: 411.» |
| 16–23 с | ski-04 | `Group discount: −10% from 11 people`<br>`Six of you: full price`<br>`6 + 5 = 11` | «The group discount starts at 11 people. Six of you pay full price. Bring five more friends.» |
| 23–30 с | ski-06 | `Rest day?`<br>`4-in-6 ticket: €317.50`<br>`4 ski days of your choice within 6`<br>`(4 × €82 = €328: small saving, more flexibility)` | «Want a rest day? The 4-in-6 ticket: 317 euros 50 for four ski days of your choice within six.» |
| 30–36 с | ski-07 или запись экрана | `Create a trip: goplanvia.com`<br>`PlanVIA: AI Group Trip Planner`<br>`Day-by-day plan · map · real places · share the plan` | «Plan the trip in PlanVIA, the AI group trip planner. Link in bio.» |

Финал: «Plan the trip in PlanVIA, the AI group trip planner. Link in bio.»

#### Подпись

```
Ski day with friends at Zillertal Arena, winter 2026/27, adult day ticket: €82 from 8:00, €78.50 from 10:30, €63.50 from 12:00, €45 from 13:30 (later start = less time on the slopes). Six friends all at 8:00: €492. Two early, two mid-morning, two after lunch: €411 (our math). Group discount starts at 11 people (10%). 4-in-6 ticket: €317.50. Season 4 Dec to 11 Apr, snow permitting.
Plan the rest of the trip day by day, with a map and real places, in PlanVIA, the AI group trip planner. Create a trip or copy a ready plan: goplanvia.com (link in bio).
Source: zillertalarena.com. Prices checked 30 Oct 2026 and may change. Visuals are AI-generated.
#SkiTrip #Zillertal #GroupTravel #TripWithFriends #SkiWithFriends
```

Shorts, заголовок: `Ski trip with friends: Zillertal Arena ticket math 2026/27`
Shorts, описание: `PlanVIA is an AI group trip planner: plan a trip with friends in minutes, with a day-by-day itinerary, a map and real places.`

### ES

#### Хук (0–2 с)
Текст на экране: `6 amigos, 1 día de esquí: 4 precios`
Голос: «Misma estación. Cuatro precios de forfait.»

#### Раскадровка

| Время | Кадр | Текст на экране | Озвучка |
|---|---|---|---|
| 2–9 с | ski-02 | `ZILLERTAL ARENA · forfait de día adulto · invierno 2026/27`<br>`desde las 8:00  82 €`<br>`desde las 10:30  78,50 €`<br>`desde las 12:00  63,50 €`<br>`desde las 13:30  45 €`<br>мелко: `temporada 4 dic – 11 abr, con nieve suficiente` | «Zillertal Arena, forfait de día para adultos, invierno 2026/27: 82 euros desde las 8:00, 45 desde las 13:30.» |
| 9–16 с | ski-03, вставка ski-05 | `6 × 82 € = 492 €` (todos a las 8:00)<br>`2 a las 8:00 + 2 a las 10:30 + 2 a las 13:30 = 411 €`<br>`¿Se une tras comer? −37 € (y esquía menos)` | «Seis amigos a las 8:00: 492 euros. Dos pronto, dos a media mañana, dos tras comer: 411.» |
| 16–23 с | ski-04 | `Descuento de grupo: −10 % desde 11 personas`<br>`Si sois seis: tarifa completa`<br>`6 + 5 = 11` | «El descuento de grupo empieza en 11 personas. Si sois seis, pagáis tarifa completa. Traed a cinco amigos más.» |
| 23–30 с | ski-06 | `¿Día de descanso?`<br>`Forfait 4 en 6: 317,50 €`<br>`4 días de esquí a elegir dentro de 6`<br>`(4 × 82 € = 328 €: poco ahorro, más flexibilidad)` | «¿Día de descanso? El forfait 4 en 6: 317,50 euros por cuatro días de esquí a elegir en seis.» |
| 30–36 с | ski-07 или запись экрана | `Crea un viaje: goplanvia.com`<br>`PlanVIA: AI Group Trip Planner`<br>`Plan día a día · mapa · lugares reales · comparte el plan` | «Organizad el viaje en PlanVIA, el planificador de viajes en grupo con IA. Enlace en la bio.» |

Финал: «Organizad el viaje en PlanVIA, el planificador de viajes en grupo con IA. Enlace en la bio.»

#### Подпись

```
Un día de esquí con amigos en Zillertal Arena, invierno 2026/27, forfait de día para adultos: 82 € desde las 8:00, 78,50 € desde las 10:30, 63,50 € desde las 12:00, 45 € desde las 13:30 (empezar más tarde = menos tiempo en pista). Seis amigos a las 8:00: 492 €. Dos pronto, dos a media mañana, dos tras comer: 411 € (nuestra cuenta). El descuento de grupo empieza en 11 personas (10 %). Forfait 4 en 6: 317,50 €. Temporada del 4 de dic al 11 de abr, con nieve suficiente.
Planificad el resto del viaje día a día, con mapa y lugares reales, en PlanVIA, el planificador de viajes en grupo con IA. Crea un viaje o copia un plan listo: goplanvia.com (enlace en la bio).
Fuente: zillertalarena.com. Precios revisados el 30 oct 2026; pueden cambiar. Imágenes generadas con IA.
#Esquí #Zillertal #ViajesEnGrupo #ViajarConAmigos #EsquiarConAmigos
```

Shorts, заголовок: `Esquí con amigos: cuentas del forfait en Zillertal Arena 2026/27`
Shorts, описание: `PlanVIA es un planificador de viajes en grupo con IA: organiza un viaje con amigos en minutos, con un itinerario día a día, un mapa y lugares reales.` (черновик, вопрос 10)

### Медиа (fal.ai, общие для EN и ES)

Пометка AI-контента: да. Суффикс к каждому промпту и правила движения те же, что в v1. Лыжников, шлемов с лицами, надписей на лыжах и кабинках нет.

| Кадр | Окно | Промпт (картинка) | Движение |
|---|---|---|---|
| ski-01 | 0–2 с | Empty chairlift chairs rising over a freshly groomed alpine slope at sunrise, pink light on snowy peaks, long shadows, no skiers. | Chairs glide up the line, slow push-in. |
| ski-02 | 2–9 с | Top-down flat lay on fresh snow: four blank rectangular lift passes in four different muted colors in a row, a plain lanyard, soft morning light. The passes are completely blank. | Cards slide in one by one from the right, snow sparkles. |
| ski-03 | 9–16 с | Six pairs of skis in different colors stuck upright in the snow in front of a wooden mountain hut, ski boots lined up beside them, morning light, skis without any brand markings. | Light snowfall, slow lateral drift. |
| ski-04 | 16–23 с | Wide alpine valley village in snow with plain white gondola cabins without lettering climbing a cable line toward the peaks, midday sun. | Gondola cabins glide, slow push-in. |
| ski-05 | вставка 2 с + запас | Mountain hut terrace in afternoon sun: empty wooden tables, two steaming cups and a thermos, folded blankets on deckchairs, snowy peaks behind. | Steam rises, shadows move slowly. |
| ski-06 | 23–30 с | Snowy mountain village at dusk, lit chalet windows, smoke from chimneys, a quiet empty street, blue hour. | Slow push-in, windows glow warmer. |
| ski-07 | 30–36 с | Soft pale-blue to white snow gradient with gentle falling snow and distant blurred peaks at the bottom, large empty space in the center for text. | Snow drifts slowly. |

---

## Что проверить фактчекеру

- Цифры извлечены инструментом WebFetch (краткий пересказ официальной страницы). Прямой curl к wien.info и nuernberg.de из среды закрыт прокси (403), поэтому исходный HTML не сверялся. Каждую цифру из таблиц выше нужно открыть вручную по ссылке.
- Расхождения, которые стоит увидеть глазами: у Нюрнберга в день открытия часы 10:00–22:00 с паузой 17:30–18:00 на церемонию; у Вены на Silvesterpfad «eight locations» против пяти карточек; в PDF Цилерталя за 2025/26 цены другие (€79 против €82), берём только 2026/27.
- Расчёты (6 × 82, 411, 37, 328 против 317,50, число выходных) проверены скриптом, но числа выходных зависят от того, что считаем «полными» выходными (сб + вс внутри дат).
- «Prices may be subject to change» у Zillertal Arena: подпись и титры предупреждают об этом. Если ролик выйдет позже 13 нояб. (v1) или после открытия сезона, актуальность цен перепроверить ещё раз.
- Цен на ярмарках (вход, залог за кружку, глинтвейн) на официальных страницах нет — в v1 их нет. Нужны для будущего ролика → `[проверить вручную]` у организаторов (Marktamt Нюрнберга, christkindlmarkt.at).

## Открытые вопросы

1. Озвучка: голос Ярослава, TTS (какой сервис и голос) или только титры? Сценарии работают во всех трёх вариантах.
2. Умеет ли продукт строить план для Вены, Нюрнберга и Zell am Ziller (входят ли в 100+ направлений) и есть ли в каталоге готовые планы по ним? Если да — дать ссылки на `/plan/<id>` для подписей, если нет — оставляем общий CTA «create a trip / copy a ready plan».
3. Запись экрана настоящего продукта (маршрут по дням с картой) для финальных кадров. Без неё работает текстовая карточка `*-07`.
4. Умеет ли Postiz при публикации проставлять метку AI-контента на TikTok / Instagram / YouTube? Если нет, ставит Ярослав вручную при публикации.
5. Для испаноязычной аудитории лыжный ролик можно сделать на испанской станции (Sierra Nevada, Baqueira). Официальные страницы цен 2026/27 из среды агента не открылись (sierranevada.es вне списка разрешённых), поэтому в этом пакете один Цилерталь на обе версии.
6. Испанская фраза о продукте в `CLAUDE.md` всё ещё черновик (вопрос 10 в `plan/questions.md`); используется в описании Shorts и в ES-озвучке «el planificador de viajes en grupo con IA», как в постах LinkedIn.

## Самопроверка по роли

- Хук в первые 2 с, 3–5 фактов с цифрами, финальный CTA «create a trip / copy a ready plan» со ссылкой goplanvia.com: да, во всех шести версиях.
- PlanVIA названо голосом и в подписи, при первом упоминании с категорией: да.
- Стоп-слова из `CLAUDE.md` и обещания несуществующих функций: не использованы.
- Каждая цена, часы, даты: источник и дата проверки 30.10.2026 в таблицах и в подписях. Нет источника: `[проверить вручную]` и этого в ролике нет.
- Люди, знаменитости, чужие логотипы в промптах fal.ai: нет. Текст и цифры рисуются титрами, не моделью.
- Ничего не опубликовано, в Postiz не ставилось, медиа не генерировалось.
