# Домашнее задание к занятию "4.1. Модель OSI/ISO. Обзор сетевых протоколов" Белов Антон
**

### Задание 1.
С помощью открытых источников попробуйте понять, в чем разница между хабом, коммутатором и маршрутизатором в разрезе уровней модели OSI?

Приведите ответ в свободной форме.

Ответ: хаб работает только на физическом уровне и не обрабатывает пакеты, при получении отправляет их на все свои активные порты.

коммутатор при получении пакета проверяет кому он адресован и отправляет его в конкретный порт. Работает в пределах одной подсети. Имеет только внутренние порты.

маршрутизатор дополнительно к коммутатору может работать с различными сегментами сети, а также сетями с другими архитектурами. Имеет как внутренние, так и внешние порты.

### Задание 2.
Какой уровень OSI отвечает за надежную доставку данных?

Приведите ответ в свободной форме.

Ответ: транспортный, в частности при работе одного из его протоколов TCP, проверяется, был ли доставлен пакет и если нет, то устройство переотправляет его заново.

### Задание 3.
Как называется процесс добавления заголовков к данным при прохождении их от одного уровня OSI к другому?

Приведите ответ в свободной форме.

Ответ: инкапсуляция, к данным при прохождении от прикладного уровня к физическому на каждом уровне добавляется соответствующий заголовок.

### Задание 4.
Какая максимальная длина ethernet-кабеля по стандарту cat5e? Какой уровень модели OSI описывает этот стандарт и ограничения, связанные с ним?

Приведите ответ в свободной форме.

Ответ: по стандарту максимальная длина ethernet-кабеля cat5e - 100м., описано на физическом уровне модели OSI.

### Задание 5.
На каком уровне/уровнях модели OSI работают следующие протоколы:

FTP - прикладной

HTTPS - прикладной

TCP - транспортный

Ethernet - канальный

JPEG - представительский

SIP - прикладной

Приведите ответ в свободной форме.

### Задание 6.
Как вы думаете, какие преимущества у подключения компьютера по Wi-Fi по сравнению с проводным соединением?

Приведите ответ в свободной форме.

Ответ: удобство использования, т.к. не нужно прокладывать дополнительных проводов между компьютером и Wi-Fi устройством, большая мобильность, поскольку с переносным компьютером можно перемещаться между комнатами в квартире. Некоторые устройства в принципе не предполагают проводное соединение, например, смартфоны и планшеты. По Wi-Fi можно получить большую скорость, чем Ethernet 100 Мбит/с, многие роутеры по Wi-Fi дают реальную скорость 300 Мбит/с и выше.

**

Дополнительные задания (со звездочкой*)
Эти задания дополнительные (не обязательные к выполнению) и никак не повлияют на получение вами зачета по этому домашнему заданию. Вы можете их выполнить, если хотите глубже и/или шире разобраться в материале.

### Кейс 7.
На каком уровне OSI работает ping?

Приведите ответ в свободной форме.
