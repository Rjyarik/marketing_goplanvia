# Фактчек: хаб «AI trip planner for friends» (/group-trip-planner, EN)

Черновик: `content/pages/2026-10-29-group-trip-planner.en.md`
Бриф: `research/briefs/2026-10-29-friends-trip-planner-hub.en.md` · задача W2-03
Фактчекер, проверено 2026-10-30. Каждое утверждение сверено с открытой страницей, сниппеты поиска как источник не использовал. Текст черновика не менял: ниже только «что на что заменить». Ссылки вида L84 указывают на строку черновика.

Вердикт: **не пропускаю** в текущем виде.

## Итог

| | Всего | pass | fix | cannot verify |
|---|---|---|---|---|
| Все проверяемые утверждения | 59 | 40 | 10 | 9 |
| Из них пометки «[проверить вручную]» в тексте | 17 | 1 | 4 | 12 |

**Может ли черновик идти Ярославу:** на одобрение публикации — нет. По `CLAUDE.md` черновик с пометкой «[проверить вручную]» дальше не идёт, а после всех возможных правок их останется до 12. Ярославу сейчас стоит отправить только вопросы (список в конце).

**Блокеры:**
1. **Секция «How much does a 3-day trip… cost»** (M2–M6). Ни одной цифры: проверенных страниц Lisbon и Porto пока нет. Фраза «Each trip below has its own estimate, checked against official prices» сейчас неверна.
2. **Цены Plus** (M13). Их надо убрать: в `plan/questions.md` п. 3 и W0-11 сказано, что оплата Plus в продукте не подтверждена и цены нигде не публикуем. goplanvia.com/plus из моей среды открыть нельзя: URL не в allowlist, в поиске сайт не индексируется.
3. **Как работает ссылка на план** (M1, M14, а также вступление, шаг 4, таблица и FAQ): нужен ответ Ярослава, `plan/questions.md` п. 2. W2-02 («открытая ссылка без регистрации») ещё в статусе todo, поэтому формулировку «drops the link in the group chat, so all six of you are looking at the same Saturday» без ответа не подтвердить.
4. **Нет раскрытия партнёрских ссылок** (L54, L146). Это требование ценности «прозрачность». Текст ждёт утверждения Ярослава, `plan/questions.md` п. 12.
5. **Кошелёк билетов** (L55, L118) намекает, что друзья видят билеты. В `CLAUDE.md` этого нет, правка ниже (п. 49).
6. **Torre de Belém и BOE** (M9–M12, M16). Официальный сайт памятника и BOE из среды не открылись. Варианты: открыть вручную в браузере или удалить эти фразы (тогда пометки уходят).
7. **Заглушки вне фактчека, которые тоже блокируют публикацию:** автор (L9, L179), цитата практика (L128), ссылки «Create a trip» (L28, L160), ссылки на планы из каталога (L75, L76, L158).

**Что подтвердилось полностью:**
- все цены и правила Pena (Parques de Sintra);
- Layla, Wanderlog, Splitwise, Tricount;
- цифры Expedia;
- цифры Google Flights: первоисточник blog.google открылся и заменяет пересказы PPC Land и 9to5Google;
- праздники Андалусии по BOJA;
- даты Semana Santa и Santo António 2027.

Запрещённых обещаний (vote, split the budget, invite your group, роли) нет. Стоп-слов нет. Бренд написан верно.

## Пометки «[проверить вручную]»: сводка

| Пометка | Строка | Что | Вердикт | Пункт таблицы |
|---|---|---|---|---|
| M1 | L60 | Ссылка на план: только просмотр, нужен ли вход | cannot verify, нужен ответ Ярослава | 45 |
| M2 | L67 | Вилка цены на человека | cannot verify | 56 |
| M3, M4 | L75 | Lisbon: цена и главная статья расходов | cannot verify | 57 |
| M5, M6 | L76 | Porto: цена и главная статья расходов | cannot verify | 58 |
| M7 | L84 | Google Flights 49 и 90 дней | fix: цифры верны, уточнить «из США» | 21 |
| M8 | L88 | Google Flights, пункт списка | fix: цифры верны, поправить формулировку | 23 |
| M9 | L96 | Belém: дни закрытия | cannot verify | 11 |
| M10 | L102 | Viernes Santo — общенациональный праздник | cannot verify по первоисточнику | 14 |
| M11 | L102 | Belém закрыта 28.03.2027 | cannot verify | 16 |
| M12 | L103 | Belém закрыта 13.06 | cannot verify | 20 |
| M13 | L134 | Цены Plus | fix: убрать цены | 51 |
| M14 | L138 | Нужен ли друзьям вход | cannot verify, нужен ответ Ярослава | 45 |
| M15 | L142 | Города с готовыми планами | pass: фраза верна, пометку снять | 54 |
| M16 | L169 | Garrigues вместо BOE | cannot verify | 29 |
| M17 | L171 | Первоисточник Google Flights | fix: первоисточник открыт | 28 |

## Проверка утверждений

### A. Места, правила посещения, даты

| # | Утверждение | Источник | Проверено | Вердикт | Что заменить |
|---|---|---|---|---|---|
| 1 | Pena: Essential visit (дворец и парк) — €20 за взрослого (L80) | [Parques de Sintra, Pena](https://parquesdesintra.pt/en/parks-monuments/park-and-national-palace-of-pena/): Adults (18–64) €20; [касса, Essential Visit](https://bilheteira.parquesdesintra.pt/info/parque-e-palacio-da-pena/1202/en): New Palace и парк | 2026-10-30 | pass | — |
| 2 | Pena: Full Tour — €45 (L80) | [Opening times and prices](https://www.parquesdesintra.pt/en/plan-your-visit/opening-times-and-prices/): «Full Tour 45 €». На странице парка он называется «Complete Visit», в кассе — [«Pena Palace: Full Visit»](https://bilheteira.parquesdesintra.pt/info/palacio-da-pena-visita-total/1376/en) | 2026-10-30 | pass | — (по желанию: «the Full Tour» → «the Full Tour (Complete Visit)», чтобы совпадало с кассой и страницей парка) |
| 3 | Билет только в парк — €12 (L80) | Opening times and prices: «Visit to the park 12 €» | 2026-10-30 | pass | — |
| 4 | Билеты во дворец на 4 человек — €80–€180 (L80) | Арифметика: 4 × €20 и 4 × €45 | 2026-10-30 | pass | — |
| 5 | Вход во дворец только в дату и время билета; раньше не пустят, опоздавших не пустят и деньги не вернут (L95) | [New tickets PNP](https://www.parquesdesintra.pt/en/plan-your-visit/new-tickets-pnp/): «There is no delay tolerance»; касса 1202: «If you arrive after your reserved time, entry will not be permitted, and your ticket will not be refunded» | 2026-10-30 | pass | — |
| 6 | От входа в парк до дворца около 30 минут (L95) | Касса 1202: «allow approximately 30 minutes between the two points» | 2026-10-30 | pass | — |
| 7 | Онлайн-билет можно перенести на другую дату в течение года (L95, L154) | New tickets PNP: «reschedule your visit date and time… within a period of one year»; opening times and prices: то же | 2026-10-30 | pass | — |
| 8 | Не публикуется, как быстро раскупают сеансы; касса помечает «Last tickets» и «Sold Out» (L95) | [Касса 263](https://bilheteira.parquesdesintra.pt/evento/parque-e-palacio-nacional-da-pena/263/en): метки «Tickets avaible», «Last tickets», «Sold Out»; срока раскупки нет | 2026-10-30 | pass | — |
| 9 | FAQ: «tickets bought online can be moved to another date within one year, but a missed slot is not refunded» (L154) | New tickets PNP: «Tickets cannot be changed or refunded in case of failure to show up at the scheduled time» | 2026-10-30 | fix: неполно. Пропущенный сеанс нельзя и перенести, а для совета про выбывших это главное | «One example: Pena Palace tickets bought online can be moved to another date within one year, but a missed slot is not refunded.» → «One example: Pena Palace tickets bought online can be moved to another date and time within one year, but only before your slot: if you miss it, the ticket can't be changed or refunded.» |
| 10 | Belém: посещение по брони на дату и время (L96) | [Turismo de Lisboa](https://www.visitlisboa.com/pt-pt/locais/torre-de-belem): бронь «data e o horário»; [Sábado/Lusa, 26.05.2026 (СМИ)](https://www.sabado.pt/gps/amp/torre-de-belem-reabre-a-brilhar-e-com-novo-sistema-de-entradas-para-reduzir-filas): слоты, до 60 человек каждые полчаса, 900 в день. Официальный сайт mosteirojeronimos.torrebelem.gov.pt не открылся | 2026-10-30 | pass: два независимых источника | — (по желанию: «Visits are booked for a date and time.» → «Since it reopened in May 2026, visits are booked for a time slot.») |
| 11 | M9. Belém закрыта по понедельникам, а также 1.01, в Пасхальное воскресенье, 1.05, 13.06 и 25.12 (L96) | Есть только у Turismo de Lisboa: «Encerrado à segunda-feira e nos dias 1 de janeiro, Domingo de Páscoa, 1 de maio, 13 de junho e 25 de dezembro». Сайт памятника (mosteirojeronimos.torrebelem.gov.pt) и касса MMP/Blueticket из среды не открылись | 2026-10-30 | cannot verify: по `CLAUDE.md` часы и выходные сверяем с официальным сайтом места | Вариант А: Ярослав или координатор открывает сайт памятника в браузере; если всё совпадает, заменить источник на официальный и снять пометку. Вариант Б: удалить фразу «It is closed on Mondays and on 1 January, Easter Sunday, 1 May, 13 June and 25 December. [проверить вручную: …]» |
| 12 | Semana Santa — с воскресенья 21 по воскресенье 28 марта 2027 (L102) | Пасха 2027 — 28 марта (расчёт по пасхалии); [BOJA № 84](https://www.juntadeandalucia.es/eboja/2026/84/BOJA26-084-00002-5812-01_00337048.pdf): Jueves Santo 25.03, Viernes Santo 26.03 | 2026-10-30 | pass | — |
| 13 | В Андалусии праздники в четверг 25 и пятницу 26 марта (L102) | BOJA № 84 от 05.05.2026, Decreto 84/2026: «25 de marzo, Jueves Santo», «26 de marzo, Viernes Santo» | 2026-10-30 | pass: первоисточник | — |
| 14 | M10. Великая пятница, 26 марта, — праздник по всей Испании (L102) | [Garrigues](https://www.garrigues.com/es_ES/noticia/publicado-boe-calendario-laboral-espana-2027) и [Cuestiones Laborales](https://www.cuestioneslaborales.es/calendario-laboral-fiestas-2027/): одна из 9 общих фиест, «festivos en toda España». Первоисточник BOE-A-2026-21254 (Resolución de 8.10.2026, BOE 13.10.2026) не открылся | 2026-10-30 | cannot verify по первоисточнику. Два вторичных источника совпадают, риск ошибки низкий | Вариант А: открыть [BOE-A-2026-21254](https://www.boe.es/diario_boe/txt.php?id=BOE-A-2026-21254) вручную и снять пометку. Вариант Б: удалить «; Good Friday (26 March) is a national holiday in Spain [проверить вручную]». Для группы и так хватает строки про Андалусию из BOJA |
| 15 | «If some of you live in Spain, Thursday to Sunday is your 4-day window.» (L102) | [El Demócrata (СМИ)](https://www.democrata.es/empleo/calendario-laboral-2027-festivos-puentes-comunidades-autonomas/): Jueves Santo — праздник «en todo el territorio salvo en Cataluña y la Comunidad Valenciana»; Lunes de Pascua 29.03 — Балеары, Каталония, Наварра, Страна Басков, Валенсия, Риоха. Для Валенсии то же пишет [El Español, 21.03.2026 (СМИ)](https://www.elespanol.com/valencia/20260321/oficial-calendario-laboral-valenciano-puentes-dias-festivos-inhabiles-trt/1003744177913_0.amp.html) | 2026-10-30 | fix: для Каталонии и Валенсии неверно, там 4 дня — с пятницы по понедельник | → «If some of you live in Andalusia, Thursday to Sunday is your 4-day window; elsewhere in Spain, check your region's calendar first.» Когда приложение к BOE откроют вручную, можно добавить: «In Catalonia and the Valencian Community, Thursday is a working day and Easter Monday (29 March) is the holiday.» |
| 16 | M11. Belém закрыта в Пасхальное воскресенье, 28 марта (L102) | Зависит от п. 11; дата Пасхи верна | 2026-10-30 | cannot verify | Как в п. 11. По варианту Б удалить «Belém Tower is closed on Easter Sunday, 28 March [проверить вручную].» и ссылку «[Turismo de Lisboa](…torre-de-belem)» в колонке Source |
| 17 | Ночь святого Антония — суббота 12 и воскресенье 13 июня 2027 (L103) | [Turismo de Lisboa, St Anthony's night](https://www.visitlisboa.com/en/events/st-anthonys-night-12-13th-june): «12 Jun – 13 Jun», каждый год; 12.06.2027 — суббота | 2026-10-30 | pass | — |
| 18 | «The peak of Lisbon's June festivities» (L103) | [Lisbon Festivities](https://www.visitlisboa.com/en/events/lisbon-festivities-1): «The festival's highlight is the parade on Avenida da Liberdade»; St Anthony's night: в эту ночь проходят Marchas Populares по Avenida da Liberdade | 2026-10-30 | pass по двум страницам | В колонку Source добавить «; [Turismo de Lisboa, St Anthony's night](https://www.visitlisboa.com/en/events/st-anthonys-night-12-13th-june)» |
| 19 | Программа на июнь 2027 — «to be confirmed» (L103) | Lisbon Festivities: «Jun 2027 (to be confirmed)» | 2026-10-30 | pass | — |
| 20 | M12. Belém закрыта 13 июня (L103) | Зависит от п. 11 | 2026-10-30 | cannot verify | Как в п. 11. По варианту Б удалить «Belém Tower is closed on 13 June [проверить вручную].» |

### B. Когда покупать билеты

| # | Утверждение | Источник | Проверено | Вердикт | Что заменить |
|---|---|---|---|---|---|
| 21 | M7. «Google Flights puts the low-price window for trips to Europe from 49 days before departure, with the average low around 90 days» (L84) | [Google, «Wheels up: Trends and tips for 2026 holiday travel», 05.10.2026](https://blog.google/products-and-platforms/products/search/holiday-travel-trends-2026/): «Trips to Europe: Like general international travel, lowest prices hit 90 days out», «The low price range is 49 days or more before departure»; данные — вылеты из США | 2026-10-30 | fix: цифры верны, но в ответе под H2 не сказано, что это вылеты из США. Читатель из Европы примет их на свой счёт | «Google Flights puts the low-price window for trips to Europe from 49 days before departure, with the average low around 90 days [проверить вручную].» → «for flights from the US to Europe, Google Flights puts the low-price range at 49 days or more before departure, with the lowest prices about 90 days out ([Google, 5 Oct 2026](https://blog.google/products-and-platforms/products/search/holiday-travel-trends-2026/)).» |
| 22 | Google Flights: октябрь 2026, данные за 5 лет, вылеты из США (L88) | Google: «Oct 05, 2026», «five years of aggregated data from Google Flights», «U.S. departures» | 2026-10-30 | pass | — |
| 23 | M8. «trips to Europe were cheapest from 49 days out, with the average low point about 90 days out» (L88) | Google: 49 дней — начало диапазона низких цен («49 days or more»), минимум — около 90 дней | 2026-10-30 | fix: формулировка «cheapest from 49 days out» неточная | «trips to Europe were cheapest from 49 days out, with the average low point about 90 days out; spring-break trips in March and April bottomed out at about 50 days. [проверить вручную: …]» → «for trips to Europe, fares were in the low range from 49 days or more before departure and lowest about 90 days out; for spring-break trips in March and April, the lowest point was about 50 days out (low range 29–64 days).» |
| 24 | Весенние каникулы, март и апрель: минимум около 50 дней (L88) | Google: «Spring break: Lowest prices hit 50 days before departure (low price range is 29–64 days)», «for trips in March or April» | 2026-10-30 | pass | — (входит в правку п. 23) |
| 25 | Expedia 2026 Air Hacks: бронирования на Expedia.com с декабря 2024 по ноябрь 2025 (L89) | [Expedia](https://www.expedia.com/newsroom/expedia-2026-air-hacks/): «based on bookings made on Expedia.com from December 2024 – November 2025» | 2026-10-30 | pass | По желанию добавить дату публикации: 17.02.2026 ([Business Wire](https://www.businesswire.com/news/home/20260217013882/en/EXPEDIA-2026-AIR-HACKS-FRIDAY-TAKES-OFF-AS-THE-CHEAPEST-DAY-TO-DEPART-AND-BOOK)) |
| 26 | Международный эконом дешевле всего за 8–15 дней (L89) | Expedia: «The most affordable time to book an international economy flight is 8 – 15 days out» | 2026-10-30 | pass | — |
| 27 | Бронь за 31–45 дней экономит около $190 по сравнению с бронью за 6+ месяцев (L89) | Expedia: «save $190 on average by booking 31 – 45 days ahead, instead of six months out» | 2026-10-30 | pass | — |
| 28 | M17. Источник Google Flights — пересказы PPC Land и 9to5Google (L171) | Первоисточник blog.google открыт, цифры совпадают | 2026-10-30 | fix: заменить на первоисточник | «- Google Flights data, as reported by [PPC Land](…) and [9to5Google](…), 5 Oct 2026 [проверить вручную: первоисточник blog.google]» → «- Google: [Wheels up: Trends and tips for 2026 holiday travel](https://blog.google/products-and-platforms/products/search/holiday-travel-trends-2026/), 5 Oct 2026» |
| 29 | M16. Источник праздников Испании — Garrigues вместо BOE (L169) | BOE-A-2026-21254 не открылся (см. п. 14) | 2026-10-30 | cannot verify | После ручной проверки BOE: «- Garrigues: […] [проверить вручную: первоисточник BOE-A-2026-21254]» → «- BOE: [Resolución de 8 de octubre de 2026, fiestas laborales 2027](https://www.boe.es/diario_boe/txt.php?id=BOE-A-2026-21254)». Если выбран вариант Б из п. 14 — удалить строку Garrigues и ссылку на Garrigues в таблице дат (L102) |

### C. Конкуренты и другие сервисы

| # | Утверждение | Источник | Проверено | Вердикт | Что заменить |
|---|---|---|---|---|---|
| 30 | Layla: AI-чат строит план «around your dates, budget and style» (L111) | [layla.ai](https://layla.ai/): «She builds it around your dates, budget and style.» | 2026-10-30 | pass | — |
| 31 | Layla: эксперты бронируют поездку; команда бронирует отели, перелёты, трансферы и активности (L111, L113, L123) | layla.ai: «Then a real travel expert checks every detail and books it»; FAQ: «our team books the arrangements included in your trip… such as hotels, flights, transfers and activities» | 2026-10-30 | pass | — |
| 32 | Layla: рекомендуемый минимум для поездок под заказ — €100 на человека за ночь (L113) | layla.ai FAQ: «recommended minimum budget of €100 per person, per night» | 2026-10-30 | pass | — |
| 33 | Layla: планирование бесплатное (L123) | layla.ai FAQ: «free, with no subscription or planning fee» | 2026-10-30 | pass | — |
| 34 | Wanderlog: добавленные места появляются на карте на основе Google Maps (L112) | [App Store, витрина США](https://apps.apple.com/us/app/wanderlog/id1476732439): «immediately pinned on your Google Maps-based travel map» | 2026-10-30 | pass | — |
| 35 | Wanderlog: «everyone can collaborate in real-time» (L60, L107, L114, L122) | App Store, США: «Like for Google Docs, everyone can collaborate in real-time.» | 2026-10-30 | pass | — |
| 36 | Wanderlog: бюджет, расходы и деление счетов в группе (L115, L122) | [wanderlog.com, expense splitting](https://wanderlog.com/travel-budget-expense-splitting-app): «Split travel expenses with friends», «who owes who»; [App Store, витрина Оман](https://apps.apple.com/om/app/id1476732439): «Set budget, track expenses, and split bills with a group». В описании на витрине США этого нет | 2026-10-30 | pass | Источник поправить в п. 40 |
| 37 | Wanderlog хранит планы офлайн в приложении (L117) | App Store, США: «stored offline on the Wanderlog travel planner app». В списке Pro (витрина Оман) офлайна нет | 2026-10-30 | pass | — |
| 38 | Splitwise бесплатен; Pro добавляет сканирование чеков, конвертацию валют и поиск по всей истории (L115, L150) | [App Store, Splitwise](https://apps.apple.com/us/app/splitwise/id458023433): «you can continue using Splitwise for free»; Pro: «OCR integration for scanning and itemizing receipts», «Convert expenses to different currencies», «Search full expense history» | 2026-10-30 | pass | — (см. замечание 2 ниже) |
| 39 | Tricount бесплатен, «no limit on tricounts or expenses» (L115, L150) | [App Store, Tricount](https://apps.apple.com/app/id349866256): «Free & unlimited – No subscription, no hidden fees, no limit on tricounts or expenses»; продавец Tricount SA | 2026-10-30 | pass | — |
| 40 | Источник Wanderlog — витрина App Store в Омане (L172) | В витрине США нет пункта про расходы, на wanderlog.com он есть | 2026-10-30 | fix: источник | «- Wanderlog: [App Store listing](https://apps.apple.com/om/app/id1476732439) <!-- … -->» → «- Wanderlog: [App Store listing](https://apps.apple.com/us/app/wanderlog/id1476732439), [budget and expense splitting](https://wanderlog.com/travel-budget-expense-splitting-app)» |

### D. Утверждения о PlanVIA

Сверка со списком «Продукт: что есть сейчас» в `CLAUDE.md`. Сайт goplanvia.com из среды не открывается (URL не в allowlist, в поиске не индексируется), поэтому всё, чего нет в `CLAUDE.md`, — «нужен ответ Ярослава».

| # | Утверждение | Источник | Проверено | Вердикт | Что заменить |
|---|---|---|---|---|---|
| 41 | Фраза о продукте (L26) | `CLAUDE.md`, «Бренд»: совпадает дословно | 2026-10-30 | pass | — |
| 42 | 100+ направлений (L3, L26, L47, L51, L111, L142) | `CLAUDE.md` | 2026-10-30 | pass | — |
| 43 | «free to start» (L26, L134) | `CLAUDE.md`: есть Plus с безлимитом планов, значит, есть бесплатный уровень; `plan/questions.md` п. 3: «пишем Freemium» | 2026-10-30 | pass, с оговоркой | Лимиты бесплатного уровня не указывать, пока нет ответа на п. 1 `plan/questions.md` |
| 44 | Каталог готовых планов: открыть, скопировать, изменить (L3, L36, L52, L111) | `CLAUDE.md` | 2026-10-30 | pass | — |
| 45 | M1, M14. Ссылка на план: друзья открывают её и видят тот же план, правит только автор (L26, L37, L53, L60, L114, L138) | Нет в `CLAUDE.md`; W2-02 (открытая ссылка без регистрации) — todo; `plan/questions.md` п. 2 | 2026-10-30 | cannot verify: **нужен ответ Ярослава** | Если ссылка открывается без входа и только для просмотра — снять обе пометки, текст оставить. Если нужен вход — L138: «Friends see the same plan; the person who built it makes the changes.» → «Friends sign in to open it and see the same plan; the person who built it makes the changes.», а в L26 после «drops the link in the group chat» добавить «(friends need a PlanVIA account to open it)» |
| 46 | Бронирование у партнёров: перелёты, поезда, аренда авто, eSIM, отели (L54, L113, L146) | `CLAUDE.md` | 2026-10-30 | pass | — |
| 47 | Раскрытие партнёрских ссылок (L54, L146) | `CLAUDE.md`, «Ценности»: «партнёрские ссылки раскрываем». Сейчас на месте текста заглушка | 2026-10-30 | fix: блокер | Заглушку «<текст раскрытия партнёрских ссылок: уточнить у координатора>» в L54 и L146 → «Some links are partner links: if you book through them, PlanVIA earns a commission at no extra cost to you.» (вариант из `plan/questions.md` п. 12, ждёт утверждения Ярослава) |
| 48 | Кошелёк билетов: брони и билеты поездки, PDF и картинки (L55, L118, L146) | `CLAUDE.md` | 2026-10-30 | pass | — |
| 49 | «so the person who booked the train isn't the only one who can find the tickets» (L55); «Everyone's tickets in the trip, not in one person's inbox» (L118) | В `CLAUDE.md` не сказано, что друзья видят кошелёк. Приглашений и ролей в продукте нет, так что фраза намекает на общий доступ, которого может не быть | 2026-10-30 | fix (если Ярослав подтвердит, что кошелёк виден по ссылке, — pass) | L55: «, so the person who booked the train isn't the only one who can find the tickets.» → «, so the trip's tickets aren't scattered across inboxes.» L118, колонка Why: «Everyone's tickets in the trip, not in one person's inbox» → «All the trip's tickets in one place, not scattered across inboxes» |
| 50 | PlanVIA Plus: безлимит планов, AI-консьерж, экспорт в PDF, офлайн (L56, L117, L134) | `CLAUDE.md` | 2026-10-30 | pass | — |
| 51 | M13. Plus стоит €4.99 в месяц, €10.99 за 3 месяца, €29.99 в год (L134) | goplanvia.com/plus не открывается. `plan/questions.md` п. 3 и W0-11: оплата Plus не подтверждена (тестовый ключ Stripe), «цены нигде не публикуем» | 2026-10-30 | fix: убрать цены | «PlanVIA Plus adds unlimited plans, an AI concierge, PDF export and offline access for €4.99 a month, €10.99 for 3 months or €29.99 a year [проверить вручную: сверить с goplanvia.com/plus].» → «PlanVIA Plus adds unlimited plans, an AI concierge, PDF export and offline access.» Цены вернуть после W0-11, со ссылкой на /plus и датой проверки |
| 52 | PlanVIA не считает, кто сколько заплатил (L47, L115, L124, L150) | `CLAUDE.md`: общего бюджета нет | 2026-10-30 | pass | — |
| 53 | Офлайн — в PlanVIA Plus (L117) | `CLAUDE.md` | 2026-10-30 | pass | — |
| 54 | M15. «Some cities also have ready-made plans in the catalogue that you can copy and change.» (L142) | `CLAUDE.md`: каталог есть | 2026-10-30 | pass: фраза верна и без списка городов | Удалить «[проверить вручную: список городов с готовыми планами — у координатора]». Список городов — по желанию, после ответа на п. 6 `plan/questions.md` |
| 55 | Нет обещаний голосования, общего бюджета, приглашений и ролей | Поиск по тексту: «vote», «invite», «split the budget», «role», «agree in one evening» — только в служебном комментарии L20. Совместное редактирование честно отдано Wanderlog | 2026-10-30 | pass | — |

### E. Сколько стоит поездка

| # | Утверждение | Источник | Проверено | Вердикт | Что заменить |
|---|---|---|---|---|---|
| 56 | M2. Вилка «€… – €…» на человека за 3 дня (L67) | Опубликованных проверенных страниц городов нет (в `data/place-facts.csv` нет ни одной цены жилья или поездки по Лиссабону и Порту) | 2026-10-30 | cannot verify: блокер | Заполнить только из проверенных страниц Lisbon и Porto. Если хаб нужно выпустить раньше, решает координатор: убрать H2 и таблицу или перестроить раздел вокруг проверенного примера Pena. По чек-листу п. 1 у H2 должен быть ответ с цифрой |
| 57 | M3, M4. Строка Lisbon: цена на человека и главная статья расходов (L75) | То же | 2026-10-30 | cannot verify | То же |
| 58 | M5, M6. Строка Porto, Semana Santa: цена и главная статья расходов (L76) | То же | 2026-10-30 | cannot verify | То же |
| 59 | «Each trip below has its own estimate, checked against official prices, and a link to copy the plan.» (L67) | В таблице нет ни одной заполненной строки | 2026-10-30 | fix: сейчас неверно | Оставить фразу, только когда в таблице будут заполненные и проверенные строки. До этого удалить |

## Утверждения о продукте

- Всё, что обещано в тексте, есть в списке «что есть сейчас»: маршрут по дням с картой и реальными местами для 100+ направлений, каталог с копированием, партнёрское бронирование, Plus (безлимит, AI-консьерж, PDF, офлайн), кошелёк билетов. Фраза о продукте совпадает дословно.
- Несуществующих функций текст не обещает: голосований, общего бюджета, приглашений и ролей нет. Совместное редактирование описано честно как то, чего нет, с отсылкой к Wanderlog.
- **Нужен ответ Ярослава:**
  - (а) как работает ссылка на план: вход, просмотр, копирование (`plan/questions.md` п. 2);
  - (б) виден ли друзьям по ссылке кошелёк билетов (новый вопрос, к п. 2);
  - (в) цены Plus и живые оплаты (п. 3, W0-11);
  - (г) текст раскрытия партнёрских ссылок (п. 12);
  - (д) планы Lisbon и Porto в каталоге (п. 6).

## Стоп-слова и бренд

- Стоп-слов нет: hidden gem, nestled, bucket list, breathtaking, vibrant, must-see, unforgettable, embark, delve, «whether you're», «fast-paced» — ни одного совпадения.
- Бренд везде написан как PlanVIA; ошибочных вариантов (Planvia, PlanVia, planvia) и домена yourplanvia.com нет. При первом упоминании указана категория. Адрес /group-trip-planner соответствует `CLAUDE.md`.
- Призывы к действию «Create a trip», «Copy this itinerary», «Browse ready-made trips» — по правилам, «Sign up» нигде нет.

## Источник и дата у каждой цифры

- **Есть:**
  - Pena (L80): ссылка и дата прямо в тексте;
  - таблица дат 2027: колонки Source и Checked;
  - таблица инструментов: строка «Checked» и раздел Sources;
  - Expedia, Layla, Splitwise, Tricount: раздел Sources с общей датой «Checked: 28 Oct 2026».
- **Нет или не тот источник:**
  - цены Plus (L134): источника нет → убрать (п. 51);
  - вилка цены и таблица городов (L67–L76): цифр нет;
  - Google Flights в ответе под H2 (L84): нет ссылки → правка п. 21 добавляет ссылку на первоисточник;
  - дни закрытия Belém: источник не официальный (п. 11).
- **Цифры-примеры:** «€300 for 3 nights», «48-hour deadline», «three cities», «six/seven people», «30 minutes earlier» — это иллюстрации к советам, не факты, источник им не нужен.
- **Даты проверки:** после правок обновить «Checked: 28 Oct 2026» (L126, L164, колонка Checked в таблице дат) и «Updated» (L8, L179) на дату финальной проверки. Повторно сверено 30.10.2026.

## Чек-лист страницы (вне фактчека, блокирует публикацию)

- п. 4: нет цитаты практика (L128).
- п. 6: нет реального автора (L9, L179), `plan/questions.md` п. 11.
- п. 7: нет ссылки на план, который открывается без регистрации (L158). Зависит от W2-02 и п. 6 вопросов.
- п. 3: таблица с цифрами пустая (п. 56–58).

## Замечания для координатора

1. **Torre de Belém после ремонта.** Башня была закрыта около года и открылась в конце мая 2026 (по разным СМИ — 26 или 27 мая). Теперь вход по слотам: до 60 человек каждые полчаса, около 900 в день; часы 09:30–17:30, последний вход в 17:00. Источники: Sábado/Lusa 26.05.2026 и [The Portugal News, 30.05.2026](https://www.theportugalnews.com/news/2026-05-30/emblematic-monument-in-portugal-to-reopen/1030166), reported, not confirmed. Для группы это полезнее списка выходных; можно добавить, когда подтвердится официальным сайтом.
2. **Splitwise.** В отзывах и пересказах пишут, что бесплатные аккаунты ограничены по числу расходов в день. В описании разработчика этого нет (reported, not confirmed). Править текст не обязательно. Если упоминать — только с этой пометкой.
3. **Google Flights.** Обе «большие» сводки по ценам (Google и Expedia) построены на данных из США. Для групп, которые летают внутри Европы, мы публичной сводки не нашли; я не искал её целенаправленно. Ответ под H2 «Start about 3 months before» держится на данных США — правка п. 21 это раскрывает.
4. **Вопрос для `plan/questions.md`.** Может ли Ярослав открыть в браузере mosteirojeronimos.torrebelem.gov.pt (выходные Torre de Belém) и [BOE-A-2026-21254](https://www.boe.es/diario_boe/txt.php?id=BOE-A-2026-21254) (Viernes Santo и региональный Jueves Santo)? Из среды агентов оба сайта не открываются. Если нет — выбрать вариант Б в п. 11 и 14.

## Что добавлено в `data/place-facts.csv`

12 строк с checked_by=fact-checker и checked_at=2026-10-30:
- правило пропущенного сеанса Pena;
- повторная сверка цен Pena с названиями билетов;
- открытие Torre de Belém после ремонта (reported);
- главное событие Festas de Lisboa;
- региональный Jueves Santo и Lunes de Pascua 2027 ([проверить вручную]);
- второй вторичный источник по Viernes Santo ([проверить вручную]);
- Google Flights по первоисточнику — Европа и весенние каникулы; заменяют строки файла 16–17;
- дата публикации Expedia;
- Wanderlog: wanderlog.com и витрина США;
- Layla: модель бронирования.

Старые строки не менял.

## Вопросы к Ярославу (через координатора)

1. Открывается ли ссылка на план без входа? Что видит друг: только просмотр или может скопировать? Видит ли он кошелёк билетов? (`plan/questions.md` п. 2)
2. Принимает ли сайт реальные оплаты Plus, и какие цены сейчас на /plus? Пока ответа нет, цены убираем. (п. 3, W0-11)
3. Утвердить текст раскрытия партнёрских ссылок. (п. 12)
4. Ссылки на планы Lisbon и Porto в каталоге. (п. 6)
5. Реальный автор с одной строкой био. (п. 11)
6. Открыть вручную сайт Torre de Belém и BOE-A-2026-21254 или согласиться удалить эти фразы (замечание 4).

## Повторная проверка 30.10

Черновик: `content/pages/2026-10-29-group-trip-planner.en.md`, draft v3 (Changelog 2026-10-30 (2) и (3)).
Фактчекер, проверено 2026-10-30. Объём задан координатором: только изменения от 30.10 (цены Plus, групповые функции, строка Lisbon, отсутствие данных рынка США) и закрытие п. 11, 16, 20. Ссылки вида L65 — строки версии draft v3.

Вердикт по изменениям 30.10: **пропускаю после правок.** Правка одна — R2 (голосования). Нести Ярославу на одобрение публикации можно после R2 и после решения по Porto. По `CLAUDE.md` три пометки «[проверить вручную]» про Porto не пускают черновик дальше (раздел 4).

### 1. Torre de Belém: п. 11, 16, 20 закрыты

museusemonumentos.pt открыл сам.

| # | Утверждение | Источник | Проверено | Вердикт |
|---|---|---|---|---|
| 11 | Закрыта по понедельникам, 1.01, в Пасхальное воскресенье, 1.05, 13.06 и 25.12 | [MMP, Torre de Belém](https://www.museusemonumentos.pt/pt/museus-e-monumentos/torre-de-belem): «Encerrado: Segundas-feiras, 1 de janeiro, domingo de Páscoa, 1 de maio, 13 de junho, 25 de dezembro»; «Terça a Domingo, das 9h30 às 17h30» | 2026-10-30 | верно (было cannot verify) |
| 16 | Закрыта в Пасхальное воскресенье, 28.03.2027 | То же; Пасха 2027 — 28 марта, пересчитал по пасхалии | 2026-10-30 | верно (было cannot verify) |
| 20 | Закрыта 13 июня | То же | 2026-10-30 | верно (было cannot verify) |
| 10 | Посещение по брони на дату и время | [MMP, нота от 20.05.2026](https://www.museusemonumentos.pt/pt/noticia-com/torre-de-belem-reabre-ao-publico): «O sistema de acesso por horários definidos (slots)», посетителей принимают с 27 мая | 2026-10-30 | верно; теперь есть официальный источник |

- Последнего входа (17:00) на странице MMP нет. Эту цифру не использовать.
- `data/place-facts.csv`: строки 60–61 (writer, MMP) подтверждены. В строке 62 по MMP подтверждены дата открытия и слоты, лимиты 60 и 900 остаются «reported». Строки 10–12 (visitlisboa.com, 28.10) этим устарели. CSV я не менял.

Сейчас этих фраз в хабе нет: автор удалил их по варианту Б (Changelog 2026-10-30, п. 8). Возвращать не обязательно. Если возвращать, то только с официальным источником:
- L95: «- **Belém Tower, Lisbon.** Visits are booked for a date and time ([Turismo de Lisboa](https://www.visitlisboa.com/pt-pt/locais/torre-de-belem)).» → «- **Belém Tower, Lisbon.** Visits are booked for a time slot, and the tower is closed on Mondays and on 1 January, Easter Sunday, 1 May, 13 June and 25 December ([Museus e Monumentos de Portugal](https://www.museusemonumentos.pt/pt/museus-e-monumentos/torre-de-belem); [reopening notice, 20 May 2026](https://www.museusemonumentos.pt/pt/noticia-com/torre-de-belem-reabre-ao-publico)).»
- L102, строка 12–13 June: в конец колонки «What it means for your group» добавить «Belém Tower is closed on 13 June.», в колонку Source — «[Museus e Monumentos de Portugal](https://www.museusemonumentos.pt/pt/museus-e-monumentos/torre-de-belem)».
- L101, строка Semana Santa, по желанию: «Belém Tower in Lisbon is closed on Easter Sunday, 28 March.» с той же ссылкой.
- Sources (L179): добавить «- Museus e Monumentos de Portugal: [Belém Tower](https://www.museusemonumentos.pt/pt/museus-e-monumentos/torre-de-belem), [reopening notice, 20 May 2026](https://www.museusemonumentos.pt/pt/noticia-com/torre-de-belem-reabre-ao-publico)».

Если фразы не возвращать, в L95 всё равно стоит заменить источник: Turismo de Lisboa → нота MMP от 20.05.2026. По роли фактчекера «нужна ли бронь» сверяют с официальным сайтом места, а он теперь открывается. На странице Lisbon так и сделано (L126). Это не блокер.

### 2. Изменения 30.10

| # | Утверждение | Источник | Проверено | Вердикт | Что заменить |
|---|---|---|---|---|---|
| H1 | Plus: €4.99 в месяц, €10.99 за 3 месяца, €29.99 в год; безлимит планов, AI-консьерж без ограничений, PDF, офлайн, приоритетная генерация; ссылка на goplanvia.com/plus и «Checked: 30 Oct 2026» (L58, L134–L142, L181) | `CLAUDE.md`: цены проверил координатор 30.10, «Оплата работает — цены публикуем»; CSV 161. Сам goplanvia.com/plus не открыл: URL не в allowlist среды | 2026-10-30 | верно по `CLAUDE.md`; п. 51 закрыт | — |
| H2 | «free to start» (L29, L134) | Как в п. 43 | 2026-10-30 | верно с оговоркой: лимит бесплатных планов не называть (вопрос 1) | — |
| H3 | По ссылке по умолчанию только просмотр; владелец даёт право редактировать и делает участником (L29, L40, L56, L113, L146, L150) | `CLAUDE.md` | 2026-10-30 | верно; п. 45 (M1, M14) закрыт | — |
| H4 | У участников общий чат, общее место для билетов и броней, голосования (L40, L50, L56, L106, L114, L116, L118, L150) | `CLAUDE.md` | 2026-10-30 | верно | — |
| H5 | Подтверждение Pena, билеты и брони кладут в общее место поездки (L94, L158) | `CLAUDE.md` | 2026-10-30 | верно | — |
| H6 | Нет общего бюджета и деления расходов; нет личного кошелька (L50, L62, L64, L124, L150, L162) | `CLAUDE.md`, «Чего пока нет» | 2026-10-30 | верно; п. 49 закрыт | — |
| H7 | «The decision itself… That's what the four steps above, and the votes, are for.» (L65) | `CLAUDE.md`: голосования есть. Что именно голосуют, не подтверждено (`plan/questions.md` п. 20, CSV 162) | 2026-10-30 | неверно: по фразе выходит, что голосованием решают «Sintra или пляж», то есть она называет предмет голосования | R2 |
| H8 | Real-time PlanVIA не приписан; про Wanderlog сказано «describes its editing as real-time» (L106, L113, L122) | `CLAUDE.md` о real-time молчит (вопрос 19); Wanderlog — App Store US, п. 35 | 2026-10-30 | верно | — |
| H9 | Ни Plus для участников, ни вход без регистрации не утверждаются | Поиск по тексту страницы | 2026-10-30 | верно | — |
| H10 | Lisbon: около €190 на человека за 3 дня без жилья, перелётов, ужинов и напитков; «Checked: 30 Oct 2026» (L69, L77, L80) | Страница Lisbon (L41, L47, L57) и пересчёт в `2026-10-30-lisbon-3-days-friends.md`, раздел «Повторная проверка 30.10»: €189,46 по строкам CSV | 2026-10-30 | верно; п. 57 (M3, M4) закрыт, п. 56 (M2) закрыт для Lisbon | N3 по желанию |
| H11 | Главная статья расходов Lisbon: «Lunches and coffee, ~€64 (the biggest priced line; the apartment is not priced)» (L77) | Строки страницы Lisbon: еда 63,90 > 50 > 32,60 > 30,96 > 12 | 2026-10-30 | верно | — |
| H12 | «so it is the same for 4 or 6 friends» (L80) | Страница Lisbon, L61: от размера группы зависит только жильё | 2026-10-30 | верно | — |
| H13 | Обе строки ведут на один план «Lisbon + Porto», и он длиннее обеих строк (L77, L78, L82, L170) | `CLAUDE.md` (план «Португалия, Лиссабон + Порту»); CSV 165 (координатор: 9+ дней) | 2026-10-30 | верно со слов координатора | — |
| H14 | Нет данных рынка США | Поиск: Google Flights, Expedia, «US», «American», вылеты из США — в тексте и Sources их нет. Ссылки apps.apple.com/us — это описания приложений, а не данные рынка | 2026-10-30 | верно | — |
| H15 | Ответ под «How far ahead…» и абзац «Flights» (L88, L90): цифры только по Pena и датам Semana Santa | CSV 6–8, 28; BOJA (п. 12–13) | 2026-10-30 | верно | — |
| H16 | Автор — Ere Jotta (L9, L189) | `CLAUDE.md`, чек-лист п. 6 | 2026-10-30 | верно; био — заглушка | — |

**R2 (L65).** «That's what the four steps above, and the votes, are for.» → «That's what the four steps above are for.» Голосования на странице и так названы в L40, L50, L56 и L114. Когда Ярослав ответит на вопрос 20, можно написать, что именно голосуют.

**N3 (по желанию), L69.** Цифра Lisbon посчитана для тех, кто в день 3 едет в Sintra; без Sintra выходит €158,50. Вариант: «In Lisbon, 3 days with friends cost about €190 per person» → «In Lisbon, 3 days with friends, with a day in Sintra, cost about €190 per person».

**N4, L73.** Служебный комментарий «Сейчас готовых 0» устарел: строка Lisbon уже заполнена. Перед публикацией убрать — HTML-комментарий может попасть в код страницы.

Стоп-слова и бренд: не найдено. PlanVIA написан верно везде, фраза о продукте (L29) совпадает дословно.

### 3. Статус вопросов из прежнего отчёта

- (а) Ссылка на план — закрыт ответом Ярослава. Открытым остаётся только вопрос «открывается ли без регистрации» (чек-лист п. 7).
- (б) Кошелёк — закрыт: у участников общее место, личного кошелька нет.
- (в) Цены Plus — закрыт.
- (г) Раскрытие партнёрских ссылок — открыт (вопрос 12).
- (д) Планы Lisbon и Porto — закрыт: один общий план.
- Замечание 4: Torre de Belém закрыто (раздел 1). BOE больше не нужен: фразу про Viernes Santo удалили.

### 4. Можно ли нести Ярославу

**Да, после R2 и решения по Porto**, в одном пакете со страницей Lisbon. Хаб ссылается на неё как на источник цифры €190; без неё ссылки в L69, L77 и L181 никуда не ведут.

Porto — три пометки «[проверить вручную]» (L69 — одна, L78 — две). Варианты:
- А: дождаться страницы Porto после фактчека (W2-05);
- Б: убрать в L69 фразу «For Porto the figure is still being checked [€… per person — проверить вручную: страница Porto, W2-05].» и строку Porto в L78. Тогда в L82 «Both rows open the same Portugal plan (Lisbon + Porto), which runs longer than either row. Copy it and keep the days you need.» → «The Lisbon row opens our Portugal plan (Lisbon + Porto), which runs longer than 3 days. Copy it and keep the days you need.»

Остаются заглушки — это решения Ярослава:
- цитата практика и имя (L128). Формально это тоже две пометки «[проверить вручную]», но координатор считает их заглушкой чек-листа п. 4;
- био Ere Jotta (L10, L189);
- раскрытие партнёрских ссылок (L57, L158, пометка «[ждёт утверждения]», вопрос 12): текст утверждает Ярослав.

Ещё открыто:
- slug страницы Lisbon: от него зависят ссылки в L69, L77 и L181;
- открывается ли план без регистрации (чек-лист п. 7). Из среды не подтвердилось: в HTML только метатеги;
- комментарий в L73 (N4).
