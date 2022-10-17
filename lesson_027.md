# Домашнее задание к занятию "4.10. DHCP, PXE" Белов Антон
**

### Задание 1.
Для чего служит протокол DHCP?

Может ли работать сеть без DHCP-сервера?

*Приведите ответ в свободной форме.*

Ответ:

Протокол DHCP служит для динамического автоматического выделения IP адресов сетевым устройствам и добавления при этом ряда опций.

Сеть может работать без DHCP, в этом случае всем участникам придется настраивать сетевые параметры вручную.

### Задание 2.
На каком порту/портах работает DHCP?

*Приведите ответ в свободной форме.*

DHCP работает на портах 67, 68 UDP

### Задание 3.
Какие настройки можно произвести используя опции?

Назовите 5.

*Приведите ответ в свободной форме.*

Ответы:

1 - маска сети

3 - маршрутизатор(ы)

6 - адреса DNS

12 - имя хоста

15 - суффикс DNS

### Задание 4.
Сконфигурируйте сервер DHCP.

*Пришлите получившийся конфигурационный файл.*

Ответ: в приложенном файле

Дополнительные задания (со звездочкой*)
Эти задания дополнительные (не обязательные к выполнению) и никак не повлияют на получение вами зачета по этому домашнему заданию. Вы можете их выполнить, если хотите глубже и/или шире разобраться в материале.

### Задание 5.
Поймайте в сети пакеты DHCP любым сниффером.

Пришлите скриншот пойманого одного пакета с объяснением что это за пакет, какой шаг получения сетевых настроек.

### Задание 6.
Сконфигурируйте сервер PXE, выложите любой образ.

Пришлите скриншот клиента, который получил настройки и подключился к PXE-серверу.