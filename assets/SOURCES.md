# Источники ресурсов LudoDrop

Кейс открывается на смотровом верстаке арктической станции. Верстак, окно и настенные металлические сетки смоделированы в Three.js. На крюках висят игровые 3D-модели из Counter-Strike 2 с оригинальными текстурами отделки. Для горного пейзажа использован ImageGen. Начальные кадры, маски окна и видеопревью каталога сняты с этой сцены. [AK-47 | Neon Rider](unseal/armory/ak-neon-rider.glb) · [AWP | Dragon Lore](unseal/armory/awp-dragon-lore.glb) · [Кадр Blacksite](unseal/courtyard/black.webp) · [Материал верстака](cases/features/bench-mat.webp) · [Горный пейзаж](cases/features/radar-horizon.webp)

Сцена стола снабжения для кошелька и нижней панели нарисована для LudoDrop с помощью ImageGen. [Стол снабжения](rooms/supply-desk.webp)

## Предметы и контейнеры CS2

Для исходных коллекций идентификаторы, модели оружия, названия покрытий, редкость и ссылки на изображения взяты из снимка ByMykel/CSGO-API от 6 ноября 2026 года. Скины и контейнеры Valve загружены с CDN Steam Community и хранятся локально. Права на игровую графику и товарные знаки принадлежат Valve и соответствующим авторам. [Проект CSGO-API](https://github.com/ByMykel/CSGO-API) · [Каталог скинов](https://raw.githubusercontent.com/ByMykel/CSGO-API/main/public/api/en/skins.json) · [Каталог контейнеров](https://raw.githubusercontent.com/ByMykel/CSGO-API/main/public/api/en/crates.json)

- В исходном наборе 900 изображений с альфа-каналом размером 512 × 384 (216 PNG и 684 WebP). Для каждого скина в каталоге указаны исходный идентификатор и локальный путь. Ножи и перчатки в интерфейсе имеют золотую редкость. [Каталог приложения](../../src/data/assets.json)
- Капсулы, наборы пинов и три дополнительные серии оружейных кейсов используют составы из каталога CS2 и локальные иллюстрации. Названия наклеек и пинов приведены по русской локализации игры. [Контейнеры](containers/) · [Каталог CS2](https://github.com/ByMykel/CSGO-API) · [Локализация Valve](https://github.com/ByMykel/counter-strike-file-tracker)
- В `cases/crate-*.png` лежат изображения контейнеров с исходными идентификаторами Valve. В LudoDrop у тематических кейсов собственные составы и цены. [Кейсы](../../src/data/cases.ts) · [Таблицы выпадения](../../src/data/drop-tables.json)
- На карточках карт используются изображения сувенирных наборов Dust II (London 2018), Ancient (Antwerp 2022), Nuke (Austin 2025), Mirage (Shanghai 2024), Inferno (Copenhagen 2024), Overpass (Berlin 2019), Vertigo (Paris 2023) и набора коллекции Anubis. Сопоставления указаны в каталоге кейсов. [Каталог кейсов](../../src/data/cases.ts) [Оригинальные контейнеры в каталоге Steam Community](https://steamcommunity.com/market/search?appid=730&category_730_Type%5B%5D=tag_CSGO_Type_WeaponCase)

## Модели и анимации открытия

Восемь кейсов мастерской созданы для LudoDrop. Изображение каждого корпуса в каталоге и его анимации открытия сняты с одной модели. Содержимое каждой серии подобрано из локального каталога игровых предметов. [Корпуса мастерской](cases/workshop/) · [Модели](unseal/models/) · [Серии и цены](../../src/data/workshop-cases.ts)

Панорама грузового депо и тематические фоны мастерской созданы для LudoDrop с помощью ImageGen. [Грузовое депо](cases/features/freight-depot.webp) · [Фоны серий](cases/workshop-backdrops/)

Помещение с металлическими стеллажами в инвентаре и каталоге предметов создано с помощью ImageGen. [Оружейная комната](cases/features/equipment-room.webp)

Панорама оружейной с подсвеченным стендом создана для инвентаря LudoDrop с помощью ImageGen. Из центральной металлической панели сделан ложемент для скинов. [Панорама](cases/features/loadout-room.webp) · [Панель](cases/features/armory-mount.webp)

Стол оперативного штаба для стенда «Контрабанды» создан с помощью ImageGen. Первый кадр «Контрабанды» снят с той же закрытой 3D-модели, которую можно повернуть в браузере. [Фон штаба](cases/features/briefing-room.webp) · [Модель на витрине](cases/features/contraband-inspect.webp)

Сцены для стенда и каталога созданы с помощью ImageGen. Для «Сломанного клыка» подготовлены панорама полевой станции Ancient, портрет оперативника и изображение корпуса по референсу 3D-модели. Фактура металлических табличек взята с поверхности стола на панораме. [Полевая станция](cases/features/ancient-outpost.webp) · [Оперативник](cases/features/outpost-operative.webp) · [Литейный цех](cases/features/foundry-yard.webp) · [Подводная станция](cases/features/deep-station.webp) · [Узел связи](cases/features/relay-station.webp) · [Лаборатория](cases/features/espionage-lab.webp)

Для CS20, «Разлома» и «Сломанного клыка» используются модели Valve с декалями серий community_24, community_26 и community_27. Капсулы и пакеты пинов имеют индивидуальную печать и объёмную анимацию в Three.js. [Модели коллекционных упаковок](../../src/collectible-model.ts)

У десяти жёлтых и трёх чёрных серий свои материалы и две игровые декали. Kilowatt и Gallery используют современный корпус, собственные эмблемы и анимацию навесного замка. Геометрия, UV, текстуры и движение взяты из локальной установки Counter-Strike 2. У eSports 2013 сделан тонкий чемодан с нижней петлёй и печатью из Steam. Восемь сувенирных наборов используют корпус `crate_aus2025_promo_de_nuke.vmdl_c` с оформлением соответствующих наборов Steam. [Модели серий](unseal/series/) · [Сувенирные наборы](unseal/models/)

У Office геометрия и механизм раскрытия взяты из модели Valve `models/props/ad_laptop/ad_laptop_animated.vmdl_c`, декаль Genesis — `community_36`. После загрузки терминала его экран перебирает предметы из пула Office и в конце подтверждает сохранённые награды. Геометрия картонной упаковки X-Ray и движущаяся плёнка созданы для LudoDrop, исходная печать взята с изображения Steam № 4668. [Терминал](../../src/terminal-model.ts) · [Упаковка X-Ray](../../src/xray-model.ts)

Девять авторских жёстких кейсов используют объёмные створки и шарниры. Для «Ронина», «Арктики», «Неонового» и «Золотого дропа» отдельно заданы размеры, огранка углов, крышки и застёжки. Панели используют графику исходных коллекций. На странице открытия серийных, авторских и сувенирных кейсов воспроизводится запись соответствующей модели с частотой 60 кадров в секунду. У «Контрабанды» тканевые стенки, подкладка и два бегунка молнии. При недоступности WebGL для сумки используется запись той же модели. [Жёсткие кейсы](../../src/hard-case-model.ts) · [Компактные корпуса](../../src/compact-case-model.ts) · [Сумка](../../src/bag-model.ts) · [Подготовка записей](../../scripts/render-inspection-fallback.mjs)

## Карты Counter-Strike 2

Кадр закрытого кейса с декалью community_27 служит референсом изображения «Сломанного клыка» на главной. При вращении кейса, капсулы или пакета браузер рисует закрытую модель в Three.js. [Изображение на стенде](cases/features/broken-fang-field.webp) · [Кадр референса](cases/features/broken-fang-inspect.webp) · [Сцена осмотра](../../src/inspection-scene.ts)

В архиве карт сохранены скриншоты и эмблемы Valve. Панорамы подготовлены в WebP шириной 1600 пикселей. Оригиналы Dust II и Nuke входят в раздел сравнения карт на сайте Counter-Strike 2. [Страница Valve](https://www.counter-strike.net/cs2)

| Карта | Исходный кадр |
| --- | --- |
| Dust II | Площадка B, вид со стороны дальней платформы. [Скриншот Valve](https://cdn.fastly.steamstatic.com/apps/csgo/images/csgo_react/cs2/maps/dust2_back_plat_s2.jpg) |
| Ancient | Двор с руинами. Ресурс локальной установки игры `panorama/images/map_icons/screenshots/1080p/de_ancient_3_png.vtex_c` из `game/csgo/pak01_dir.vpk`. |
| Nuke | Площадка A в реакторном зале. [Скриншот Valve](https://cdn.fastly.steamstatic.com/apps/csgo/images/csgo_react/cs2/maps/nuke_default_s2.jpg) |

Эмблемы карт взяты из того же игрового архива. Встроенные SVG из ресурсов `panorama/images/map_icons/map_icon_de_{dust2,ancient,nuke}.vsvg_c` растрированы в прозрачные WebP размером 192 × 192. [Изображения карт и эмблемы](maps/)

## Авторские иллюстрации

В архиве иллюстраций находятся авторские сцены 36 кейсов, созданные с помощью ImageGen. Каждый кадр содержит контейнер и окружение и хранится в `cases/scenes/<id-кейса>.webp`. Для двух коллекций также созданы панорамные иллюстрации. [Промпты сцен](cases/scenes/prompts.json)

| Коллекция | Панорама и карточка |
| --- | --- |
| Ронин | [Флагманская панорама](cases/ronin-hero.webp) · [Лаковый сундук с белой маской ханъя](cases/scenes/original-ronin.webp) |
| Ночной порт | [Портовая панорама](cases/night-port-hero.webp) · [Контейнер на причале](cases/scenes/night-port.webp) |

### Исходные предметные рендеры

На карточках десяти авторских коллекций используются их предметные рендеры с прозрачным фоном. Для «Ночного порта» на главной также используется широкая панорама причала.

| Коллекция | Файлы |
| --- | --- |
| Ночной порт | [Сцена в порту для главного экрана](cases/night-port-hero.webp) и [отдельный кейс с эмблемой якоря](cases/collections/night-port.webp) |
| Красная линия | [Карбоновый кейс с алыми рёбрами и эмблемой](cases/collections/redline.webp) |
| Неоновый, Арктика, Золотой дроп, Сакура | Исходные PNG в `cases/custom/`, WebP в `cases/collections/`. [Промпты](cases/custom/prompts.json) |
| Asiimov, Ронин, Граффити, Контрабанда | Исходные PNG в `cases/originals/`, WebP в `cases/collections/`. [Промпты](cases/originals/prompts.json) |

Промпт иллюстрации «Красная линия» приведён ниже.

> Use case: product-mockup. Create one premium photorealistic product inventory cutout of a CS2 collectible weapons crate, landscape 3:2. The Redline crate is a wide, compact rugged dark carbon-fiber equipment trunk with lacquer scarlet corner guards, red metal runners, fine parallel red stripes and an inlaid sharp diagonal triple-slash red emblem on its front. Machined titanium catch latches, carry grip in the lid, subtle use wear, beautiful black carbon weave. Three-quarter front view with the right side visible, slightly elevated camera. The whole object centered and fully visible, fills 88% of image width. Readable, carefully lit carbon surfaces, large bold red highlights, bright softbox illumination; industrial premium store catalog look. Transparent background, clean alpha contour, no floor, no separate shadow, no people, no gun, no lettering, no words, no additional objects or frame.

Четыре квадратных обложки первого ряда созданы отдельно для карточек каталога. Широкие панорамы используются на страницах кейсов. [Обложки коллекций](cases/covers/)

## Шрифты

Шрифты установлены локально из Google Fonts и распространяются по SIL Open Font License 1.1. Для кириллицы и латиницы подключаются отдельные файлы WOFF2.

| Семейство | Назначение и лицензия |
| --- | --- |
| [Inter](https://fonts.google.com/specimen/Inter) | Основной текст нового интерфейса. [OFL](fonts/inter-OFL.txt) |
| [Roboto Condensed](https://fonts.google.com/specimen/Roboto+Condensed) | Заголовки и крупные цифры. [OFL](fonts/roboto-condensed-OFL.txt) |
| [Oswald](https://fonts.google.com/specimen/Oswald) | Афишные заголовки коллекций. [OFL](fonts/oswald-OFL.txt) |
| [Onest](https://fonts.google.com/specimen/Onest) | Гарнитура исходного проекта. [OFL](fonts/onest-OFL.txt) |
| [Unbounded](https://fonts.google.com/specimen/Unbounded) | Акцидентная гарнитура исходного проекта. [OFL](fonts/unbounded-OFL.txt) |

Гравированный дракон в шапке и боковой панели создан для LudoDrop с помощью ImageGen. [Текстура металла](cases/engraved-dragon.webp)

Панорамные сцены игровых режимов созданы для LudoDrop с помощью ImageGen. На обложках изображены [калибровочный механизм](rooms/upgrade.webp), [взлётная полоса](rooms/crash.webp), [механическое колесо](rooms/wheel.webp), [кристалл в геологической лаборатории](rooms/mines.webp) и [чемодан с документами](rooms/contracts.webp).

## Звуки

Короткие семплы открытия замка, щелчка и раскрытия предмета взяты из локальной установки Counter-Strike 2. Web Audio синтезирует сигнал остановки, дополнительные низкие тоны для редкого дропа и короткие звуки действий. Пути к оригинальным игровым ресурсам и контрольные суммы PCM указаны в реестре звуков. [Источники WAV](audio/SOURCES.md) · [Манифест](audio/manifest.json)

## Стоимости

Цены сопоставлены по точному `market_hash_name` со снимком Market.CSGO от 6 ноября 2026 года, 12:30:16 UTC. Для трёх наклеек использованы отдельные предложения Skinport от 20 ноября 2026 года. В таблице у них указаны источник и дата. Игра использует их как фиксированные стоимости в виртуальных кредитах. Исходное предложение в рублях, число листингов и округлённая стоимость в кредитах сохранены для каждого предмета. [Использованный снимок](../../src/data/price-snapshot.json) · [Исходный API](https://market.csgo.com/api/v2/prices/RUB.json)


