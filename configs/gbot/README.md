## Оглавление

* [Gbot](#gbot)
* [Цена](#Цена)
* [Требования к серверу](#Требования-к-серверу)
* [Ошибки программы](#Ошибки-программы)
* [Образец конфига](#Образец-конфига)
* [Стратегии](#Стратегии)
  * [Стратегия “Линии Боллинджера”](#Стратегия-Линии-Боллинджера)
  * [Стратегия усреднения для растущего рынка «One Buy a lot Sell» (Одна большая покупка и много мелких продаж)](#Стратегия-усреднения-для-растущего-рынка-one-buy-a-lot-sell-Одна-большая-покупка-и-много-мелких-продаж)
  * [Стратегия усреднения для падающего рынка «One Sell a lot Bay» (Много мелких покупок, одна продажа всего накупленного)](#Стратегия-усреднения-для-падающего-рынка-one-sell-a-lot-bay-Много-мелких-покупок-одна-продажа-всего-накупленного)
  * [Стратегия “Скальпер”](#Стратегия-Скальпер)
* [Кто запускал конфиги, скажите есть профит?](#Кто-запускал-конфиги-скажите-есть-профит)
* [Кто может научить настраивать Gbot](#Кто-может-научить-настраивать-gbot)
* [Сводная информация по всем ботам, биржам и данному проекту "Крипто глупости"](/README.md)

# Gbot

Терминальный бот от российского разработчика. Зарекомендовал себя в первую очередь стабильностью, быстрой реакцией разработчика на доработки, минимальными требованиями к ресурсом и возможностью управления через телеграм.

* [Официальный сайт бота Gbot](https://gbot-trader.herokuapp.com)
* [Официальный readme Gbot](https://github.com/steeply/gbot-trader/blob/master/readme_ru.md)
* [Официальный FAQ Gbot](https://github.com/steeply/gbot-trader/blob/master/faq_ru.md)
* [Телеграм-канал технической поддержки Gbota](https://t.me/gbottrader_chat)
* Реферальный код при покупке Gbot: CryptoStupidity. Укажите и это поможет поддержать проект "Крипто глупости" и переодически мотивировать нас, выкладывать свежие конфиги. Заранее спасибо!
* [Сравнительная таблица по ботам](https://docs.google.com/spreadsheets/d/1VMG21PQHvU3cDLZ6fLL17TWjiEgWzSpRfk3jA37MMUg/edit?usp=sharing) где Gbot занимает одну из лидирующих позиций. Рекомендуем к применению.

Тесты на самопроверку по знанию Gbot:

* [Проверка минимальных знаний](https://docs.google.com/forms/d/e/1FAIpQLScNYnvyNwcVktCdiYjuY03nZOZczlRE-I39SUS3LEtlrbyJvA/viewform)
* [Проврка на знание команд конфига](https://docs.google.com/forms/d/e/1FAIpQLSdrfoZHqFh-D7EVy6EjaAkGnJ-9LxvoSusVSyH_-RtTECXwtw/viewform)
* [Проверка на понимание работы стратегий](https://docs.google.com/forms/d/e/1FAIpQLScvOuiwagILeM11tcyZcgPgV9SiqipOTPshhHcN0wsegriskQ/viewform)

## Цена

Бот стоит 30$ в месяц аренды на одну биржу, но есть демо-режим, который полностью функциональный и ограничивает вас суммой торговли 0.05 BTC, на текущий момент времени это ~ 900 $. Поэтому если ваше депо больше 1000 $, то вы сможете оплатить 30$ за бота, а если меньше, то и покупать бота не нужно, торгуйте демо, как только ваше депо превысит 1000 $ вы сможете арендовать бота.

Еще одно ограничение демо-режима, бот торгует только в тех парах где есть BTC, например USDT-BTC, LTC-BTC, ETH-BTC, а вот в парах USDT-LTC или LTC-ETH бот в демо-режиме торговать не будет.

## Требования к серверу

Бот терминальный и не требует много ресурсов, хватит самого дешевого сервера с тарифным планом ~5$ в месяц, либо домашнего компьютера, который вы готовы оставить работать круглосуточно. Рекомендуемые требования к компьютеру от разработчиков программы:

* Версия Node.js 8 или выше.
* Версия Npm 5 или выше. (Кроме версии 5.4.x)
* Процессор i3 2.3Ghz или выше
* Оперативная память 100mb
* Место на диске 50mb
* Доступ в интернет

## Ошибки программы

Gbot один из самых надежных ботов на рынке, который отлично себя зарекомендовал, как бесперебойный на длительном отрезке времени. Мы не встречали ситуации, когда бот закрылся с ошибкой, если у вас случится такая ситуация, обязательно напишите нам, мы свяжемся с разработчиком и поможем вам.

## Образец конфига

Образцы конфига выложены в папке бота. Если вы мечтаете скачать конфиг, запустить его, а утром проснуться с доходом +100500 денег, то вынуждены разочаровать. Такого конфига нет и никогда не будет, можно сформировать конфиг на довольно долгосрочную работу, но его доходность будет находится в пределах +5% в месяц. В любом случае потребуется ваше ежедневное участие в работе бота и его контроль и корректировка работы. Мы не рекомендуем запускать такой конфиг, так как он может вместо прибыли принести убытки.

После того как скачали файл конфига:

* Разместите файл bat в туже папку где лежит файл gbot
* Измените в файле путь cd C:\allgbot\bb-btc-usdt на ваш собственный
* Скорректируйте настройки батника под валютную пару, ситуацию на рынке
* Двойным кликом запустите файл bb.bat

## Стратегии

### Стратегия “Линии Боллинджера”

Очень рискованная стратегия, которая на нисходящем тренде будет работать в минус, так как не учитывает такое понятие, как “доходность” (профит), т.е. в этой стратегии вы не можете задать “Профит = 1%”. Бот выставляет ордера на покупку и продажу основываясь на индикаторах “Линии Боллинджера” + RSI. Подробнее о работе  можно узнать у нас в [видеоуроках на ютуб-канале “Крипто глупости”](https://www.youtube.com/watch?v=r688aZScniI&list=PLbYtQ6_YnkBQUyMXAqXzvBpFUJ9q3hn_I) всего 13 видеоуроков.

[Образец bat файла](/configs/gbot/bb_12052018.bat) для стратегии "Линии Боллинджера". Внимание! Запускать только на растущем рынке. Лучше не использовать и точно не использовать новичкам!

### Стратегия усреднения для растущего рынка «One Buy a lot Sell» (Одна большая покупка и много мелких продаж) 

Если вы видите растущий тренд, то запускайте именно данную стратегию, название говорит само за себя. Бот сделает покупку на всё депо и будет на росте продавать частями, тем самым увеличивая доход.

[Образец bat файла](/configs/gbot/ob_12052018.bat) для стратегии "Покупка одним ордером и продажа по чуть-чуть на росте". Рекомендуется запускать только когда ждёте существенного роста. Если рынок сменит тренд на нисходящий, конфиг приведёт к накоплению второй монеты. Не рекомендуем запускать новичкам.

### Стратегия усреднения для падающего рынка «One Sell a lot Bay» (Много мелких покупок, одна продажа всего накупленного)

Большая часть начинающих трейдеров не торгуют на падающем рынке, но нет ничего более доходного, чем падающий рынок. Как раз для это ситуации реализована данная стратегия, бот выставляет много ордеров вниз от текущей цены, тем самым скупая монеты при падении по самой выгодной цене, а затем когда курс возвращается на уровень начала падения - продаёт одним ордером всё закупленное.

Посмотрите [видео о том, как нужно работать на падающем рынке](https://youtu.be/zfGD0O6KhEk).

[Образец bat файла](/configs/gbot/os_12052018.bat) для стратегии "Много мелких покупок, продажа всего накупленного одним ордером". Самая безопасная стртегия. Рекомендуется для торгов на любом рынке и любых парах. Новичкам следует начинать именно с этой стратегии.

### Стратегия “Скальпер”

Когда на рынке флет или боковое движение и курс колеблется в пределах определенного “коридора” данная стратегия выставляет одновременно ордера и на покупку и на продажу. Как только рынок начинает расти вверх или падать, данную стратегию необходимо выключить.

[Образец bat файла](/configs/gbot/scalper_12052018.bat) для стратегии "Скальпер". Внимание! Запускать только на флете (боковое движение). Не учитывает профит. Лучше не использовать и точно не использовать новичкам!

###  Кто запускал конфиги, скажите есть профит?

Профит есть, но важно понимать, что конфиги выложенные на данном сайте, в группе “Крипто глупости” формировались под конкретную ситуацию на рынке и на непродолжительное время. Не каждый конфиг из этой группы можно запустить в любой момент времени и ждать дохода. Для начала изучите бота и его стратегии, если тратить время на это жалко, то [приходите на тренинг](http://cryptostupidity.com/), мы всему научим в сжатые сроки.

## Кто может научить настраивать Gbot

В рамках проекта "Крипто глупости" каждого 15-го числа месяца запускается трениннг "Автоматическая и ручная торговля на крипто бирже". [Узнайте о нём подробней](/README.md#Обучение).
