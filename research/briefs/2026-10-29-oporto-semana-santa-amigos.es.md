# Бриф: Semana Santa en Oporto con amigos

- Тип: маршрут (сезонный)
- Язык: ES, для испанского рынка. Писать текст для испанской компании, а не переводить английский: свои примеры, местные реалии, расстояния от городов Испании
- URL: /es/itineraries/semana-santa-oporto-amigos. Структуру ES-адресов уточнить у разработчика
- Главный запрос: **Semana Santa en Oporto** (+ «con amigos»)
- Для кого: 4–6 друзей 25–32 лет из Мадрида, Галисии, Кастилии и Леона, Андалусии; бюджет средний. Едут общей машиной или летят
- Сезон публикации: конец ноября 2026 — январь 2027, за 2–4 месяца до поездки. Даты поездки: 21–28 марта 2027
- Задача в backlog: W2-05 · выдача снята 28.10.2026

## Календарь, на котором держится страница

Даты посчитаны по пасхалии, но автор подтверждает каждую по официальным источникам из таблицы «Факты».

| Дата | День | Что значит для группы |
|---|---|---|
| 21.03.2027 | воскресенье | Domingo de Ramos, начало Semana Santa |
| 25.03.2027 | четверг | Jueves Santo: выходной в большинстве CCAA, выезд в среду вечером или в четверг утром. В Португалии рабочий день |
| 26.03.2027 | пятница | Viernes Santo: выходной и в Испании, и в Португалии (Sexta-feira Santa). Часы работы мест могут меняться |
| 28.03.2027 | воскресенье | Pascua. **В эту же ночь переводят часы на летнее время**: в день возвращения на час меньше |
| 29.03.2027 | понедельник | Lunes de Pascua: выходной только в части CCAA, у кого-то в группе может оказаться лишний день |

Португалия живёт на час позже материковой Испании. Это стоит учесть для бронирований и последнего поезда.

## Запросы

| # | Запрос | Интент | Где спрашивают | Объём |
|---|---|---|---|---|
| 1 | Semana Santa en Oporto | сезон, город | Google | объём не проверен |
| 2 | Oporto en Semana Santa 2027 | сезон | Google | объём не проверен |
| 3 | qué hacer en Oporto en Semana Santa | идеи | Google, ChatGPT | объём не проверен |
| 4 | viaje a Oporto con amigos | группа | Google | объём не проверен |
| 5 | Oporto en 4 días itinerario | маршрут | Google | объём не проверен |
| 6 | cuánto cuesta un viaje a Oporto 4 días | стоимость | Google, ChatGPT | объём не проверен |
| 7 | cómo ir a Oporto desde Madrid (coche, avión, bus) | логистика | Google | объём не проверен |
| 8 | peajes en Portugal con coche español | логистика | Google | объём не проверен |
| 9 | procesiones Semana Santa Braga | событие | Google | объём не проверен |
| 10 | excursión de Oporto a Braga en tren | маршрут | Google | объём не проверен |
| 11 | qué tiempo hace en Oporto en marzo | сезон | Google | объём не проверен |
| 12 | qué cierra en Portugal el Viernes Santo | факт | Google, ChatGPT | объём не проверен |
| 13 | planificar Semana Santa con amigos | группа | ChatGPT | объём не проверен |
| 14 | «Somos 5 amigos de Madrid, ¿cómo organizamos 4 días en Oporto en Semana Santa con unos 400 € cada uno?» | маршрут, разговорный | ChatGPT | объём не проверен |

Пересекается с промптами AI-замера `es-03` и `es-09` из `data/ai-visibility-prompts.csv`.

## Вопросы для H2

1. **¿Cuánto cuesta la Semana Santa en Oporto para 4 amigos?** Итог на человека: отдельно для поездки на машине и для перелёта. Сразу под ответом таблица.
2. **¿Cómo llegar a Oporto desde España: coche, avión, tren o autobús?** Время в пути и цена на человека из Мадрида, Виго и Севильи. Для машины: электронные платные дороги в Португалии, и правда ли, что на части бывших SCUT плату отменили. Плюс DGT: операции «salida» и «retorno».
3. **¿Qué abre y qué cierra en Oporto el Viernes Santo y el Domingo de Pascua?** Список проверенных часов для мест из маршрута; что бронировать заранее.
4. **¿Merece la pena ir a Braga a ver las procesiones?** Около часа поездом. Какие процессии идут вечером в четверг и в пятницу, когда последний поезд обратно. Это вечер по правилу 70/30: кто хочет — едет, остальные идут в погреба Гайи.
5. **¿Qué tiempo hace en Oporto a finales de marzo y qué hacer si llueve?** Климатическая норма IPMA (температура, дни с дождём) и план B под крышей на каждый день.

**Дни (H2), черновик логики, места и порядок уточнит автор:**
- Día 1 (jueves 25): приезд, Ribeira, мост Dom Luís I, погреб в Vila Nova de Gaia. Вечер по желанию — процессия в Браге.
- Día 2 (viernes 26, festivo en Portugal): долина Дору на поезде CP до Pinhão или Régua (в праздник проверить расписание) или Foz и Matosinhos с морепродуктами.
- Día 3 (sábado 27): центр — Clérigos, Livraria Lello (вход по брони), Mercado do Bolhão; закат в Jardim do Morro.
- Día 4 (domingo 28, Pascua + перевод часов): поздний завтрак и выезд пораньше из-за «operación retorno».

**Именованное правило PlanVIA** (выбрать одно):
- **70/30**, как сквозное правило: вечер в Браге — это и есть те самые 30%.
- **Regla del Viernes Santo**: всё, что в пятницу может закрыться или выйти на праздничные часы, бронируем до четверга.

**Цитата практика:** гид в Порту, который водит испанские группы, или организатор поездок для молодёжи и университетов из Галисии.

## Что в таблице с цифрами

Считаем на человека, два столбца: группа из 4 и группа из 6. Ориентир — выезд из Мадрида.

| Concepto | Por persona (grupo de 4) | Por persona (grupo de 6) | Fuente | Comprobado |
|---|---|---|---|---|
| Madrid–Oporto en coche, ida y vuelta (gasolina + peajes, dividido) | | | portugaltolls.com; калькулятор расхода с датой | Nov 2026 |
| Madrid–Oporto en avión, ida y vuelta, если брать в январе | | | сайты авиакомпаний, снимок цены с датой | |
| Madrid–Oporto en autobús | | | alsa.es; flixbus.es | |
| Apartamento, 3 noches | | | выборка Booking и Airbnb на 25–28.03.2027 с датой снимка | |
| Tasa turística, 3 noches | | | porto.pt | |
| Andante: metro desde el aeropuerto + 3 días | | | metrodoporto.pt | |
| Visita a una bodega en Gaia con cata | | | официальные сайты погребов | |
| Livraria Lello + Torre dos Clérigos | | | livrarialello.pt; torredosclerigos.pt | |
| Tren a Braga o al Douro, ida y vuelta | | | cp.pt | |
| Comidas, 4 días | | | меню с официальных сайтов 3–4 мест | |
| **Total (coche / avión)** | ~€… | ~€… | | |

## Факты, которые надо проверить

| Факт | Где проверять |
|---|---|
| Праздники Испании 2027: Jueves Santo, Viernes Santo, Lunes de Pascua по CCAA | BOE (resolución de fiestas laborales 2027); бюллетени автономий |
| Праздники Португалии 2027: Sexta-feira Santa 26.03, Páscoa 28.03 | diariodarepublica.pt; gov.pt |
| Перевод часов 28.03.2027 | BOE (calendario de cambio de hora) |
| Туристический сбор в Порту. По rr.pt — €3 за ночь с 01.12.2024, обсуждалось повышение. Не проверено | porto.pt |
| Andante: тарифы по зонам, метро из аэропорта (линия E) | metrodoporto.pt |
| Поезда CP Porto–Braga: время в пути, цена, **последний поезд** после процессий | cp.pt |
| Linha do Douro: Porto–Régua/Pinhão, расписание 26.03 (праздник) | cp.pt |
| Поезд Vigo–Porto (Celta): расписание и цена | cp.pt; renfe.com |
| Автобусы Madrid–Porto | alsa.es; flixbus.es |
| Прямые рейсы в Порто из Мадрида, Барселоны, Валенсии, Севильи | ana.pt (Aeroporto do Porto); сайты авиакомпаний |
| Электронные платные дороги: как платить с испанскими номерами, принимается ли Via-T, какие участки бывших SCUT бесплатны с 2025 | portugaltolls.com (Infraestruturas de Portugal); viaverde.pt |
| Operación especial Semana Santa 2027 | dgt.es |
| Программа Semana Santa в Браге 2027: названия процессий, дни, время, маршрут | diocese-braga.pt (официальная брошюра программы); cm-braga.pt |
| Livraria Lello: цена, бронь, часы на Пасху | livrarialello.pt |
| Torre dos Clérigos: цена, часы | torredosclerigos.pt |
| Погреба в Гайе (Taylor's, Graham's, Cálem, Sandeman и др.): цена дегустации, праздничные часы, бронь для 6 | официальные сайты погребов |
| Mercado do Bolhão: часы в субботу, воскресенье и праздники | mercadobolhao.pt |
| Serralves, Palácio da Bolsa: часы на Пасху | serralves.pt; palaciodabolsa.com |
| Климат конца марта: температура, дни с дождём | ipma.pt (normais climatológicas) |
| Пасхальные события 2027 в WOW Porto | wow.pt |
| Традиция Compasso Pascal в воскресенье на севере Португалии | местный официальный источник (porto.pt, diocese do Porto) |
| Документы: испанцам хватает DNI, Tarjeta Sanitaria Europea | exteriores.gob.es; seg-social.es |

## Что в выдаче и AI-ответах сейчас

Выдачу смотрел через WebSearch 28.10.2026. Это индекс США, а не google.es, поэтому для испанского рынка позиции особенно ориентировочные. Ответы AI-ассистентов не проверены, W1-04 заблокирован.

- **Слабая выдача по главному запросу.** И по «Semana Santa en Oporto con amigos», и по «qué hacer en Oporto en Semana Santa» наверху [заметка Forbes España от 03.04.2025](https://forbes.es/?p=671751) — промо пасхальных событий в WOW Porto: шоколад, бранч за €38, пары шоколада с портвейном за €40. О поездке там ничего: ни дороги из Испании, ни жилья, ни процессий. Рядом форумы losviajeros, idealista.pt/es о традициях Semana Santa в Португалии (Брага) и lisboasecreta. Страницы, которая отвечает «Semana Santa + Oporto + grupo», в выдаче не нашёл.
- **[Mochileando por el Mundo — «Oporto en 3 días: el mejor itinerario»](https://www.mochileandoporelmundo.com/3-dias-en-oporto-itinerario/)**, обновлена 06.08.2026 — классический испанский блог. Есть маршрут на 3 дня с картой, третий день — выезд (Aveiro, Braga, Douro). Почти нет цен (одна: bifana за €2,5), нет дороги из Испании, нет Semana Santa, нет советов группе. Монетизация — партнёрские ссылки Civitatis, GetYourGuide, Booking.
- **[Layla ES — «Escapada de 3 días en Oporto con amigos»](https://layla.ai/es/trip/escapada-de-3-d%C3%ADas-en-oporto-con-amigos/01JRQ6ETQSME2924GSMTB0JF5J)** — AI-сгенерированная поездка: даты 3–6 июля, 20 человек, вылет из Валенсии. Цен нет («total para 20 personas» пустой), платные места помечены «Gratis», в заголовке 3 дня, а внутри 4. Про Пасху ничего.

**Чего не хватает группе:** календаря 2027 (у кого выходной в понедельник, перевод часов в Пасху); цены на человека для машины и для самолёта; ответа про платные дороги для испанских номеров; что открыто в Viernes Santo; Браги как вечера по желанию с последним поездом; плана B на дождь.

## Угол PlanVIA

**Semana Santa 2027 в Порту для компании, с настоящим календарём.** Точные дни и что они значат для группы, цена на человека для 4 и 6 друзей (машина против самолёта), платные дороги, проверенные часы на Viernes Santo и Pascua, Брага по правилу 70/30, план B на дождь. План копируется в PlanVIA.

Не обещаем: голосование, общий бюджет, приглашения. Пишем «comparte el plan con tu grupo», «copia este itinerario».

## Маршрут или шаблон PlanVIA

<план из каталога: уточнить у координатора>

Нужен план «Oporto, 4 días» с логикой дней из этого брифа: четверг–воскресенье, Viernes Santo, Брага по желанию. Интерфейс должен открываться на испанском.

## Метаданные (черновик)

- Title (59 символов): `Semana Santa en Oporto con amigos: plan de 4 días | PlanVIA`
- Description (141 символ): `Oporto del 25 al 28 de marzo de 2027 en grupo: ruta día a día, mapa, coste por persona, qué abre el Viernes Santo y cómo llegar desde España.`
- Заголовок превью: `Semana Santa en Oporto con amigos`
- Подзаголовок превью: `Ruta, mapa y costes para tu grupo`

## Заметки координатору

- Фразы о продукте на испанском в `CLAUDE.md` нет, есть только английская. Нужна утверждённая ES-версия для первого упоминания, например «PlanVIA, el planificador de viajes en grupo con IA». Её надо утвердить, а не придумывать автору.
- В Lunes de Pascua (29.03) в одной компании выходной будет не у всех. Это хорошая тема для ролика или поста про групповую динамику, только для соцсетей.
