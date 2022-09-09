# Домашнее задание к занятию "4.3. L3-сеть" Белов Антон
**

### Задание 1.
Сколько доступно для назначения хостам адресов в подсети /25?
А в подсети с маской 255.248.0.0.
Примечение: постарайтесь потренироваться в ручных вычислениях чтобы немного набить руку, не пользоваться калькулятором сразу.

*Приведите ответ в свободной форме.*

Ответы: В подсети с маской /25 хостам можно назначить 2^7-2 = 126 IP адресов.
В подсети с маской 255.248.0.0 хостам можно назначить 2^19-2 = 524286 IP адресов.

### Задание 2.
В какой подсети больше адресов, в /23 или /24?

*Приведите ответ в свободной форме.*

Ответ: В подсети с маской /23 вдвое больше адресов, чем в подсети с маской /24. Каждая следующая/предыдущая маска увеличивает/уменьшает количество адресов в два раза.

### Задание 3.
Получится ли разделить диапазон 10.0.0.0/8 на 128 подсетей по 131070 адресов в каждой?
Какая маска будет у таких подсетей?

*Приведите ответ в свободной форме.*

Ответ: Да, диапазон 10.0.0.0/8 можно поделить на 128 (2^7) подсетей по 131070 адресов в каждой, маска у этих подсетей будет /15.

### Задание 4.
С помощью дополнительных материалов укажите минимальную маску для подсети, в которой находится:

12 хостов /28 или 255.255.255.240

39 хостов. /26 или 255.255.255.192

2 хоста. /30 или 255.255.255.252

4 хоста. /29 или 255.255.255.248

Примечение: потренируйтесь указывать маску как в формате 255.255.255.0, так и в формате /24.

*Приведите ответ в свободной форме.*

Ответы: Добавил в задание.

### Задание 5.
Используя свои знания про L2 и L3, поразмышляйте:

получится ли отправить пакет с компьютера 192.168.1.2 на компьютер 192.168.1.3 если они подключены согласно приведённой ниже схеме?

![image](https://user-images.githubusercontent.com/107868869/188731352-d2cfb8ea-0fc5-46b5-adc7-0290ab737e7f.png)

*Дайте максимально развернутый ответ.*

Ответ: При такой схеме отправить пакет с 192.168.1.2 на 192.168.1.3 не получится, т.к. маршрутизатор 192.168.1.1 его не отправит на внешний интерфейс, поскольку сеть 192.168.1.0 у него уже анонсирована как внутренняя и он будет искать 192.168.1.3 только внутри.

### Задание 6.
Используя свои знания про маску подсети, L2 и L3, ответьте на вопросы:

- смогут ли общаться между собой компьютеры 192.168.1.25/24 и 192.168.1.2/30? Нет, не смогут, т.к. 192.168.1.25 не входит в диапазон маски второго компьютера 192.168.1.2/30
- сможет ли выйти в интернет компьютер 192.168.1.25/24, если шлюзом прописан маршрутизатор 192.168.1.1? Да, сможет, т.к. 192.168.1.1 входит в диапазон 192.168.1.25/24
- сможет ли выйти в интернет компьютер 192.168.1.2/30, если шлюзом прописан маршрутизатор 192.168.1.1? Да, сможет, т.к. 192.168.1.1 входит в диапазон 192.168.1.2/30

![image](https://user-images.githubusercontent.com/107868869/188732570-60a2d1aa-4c4b-480d-8e9e-8b8c78002ceb.png)

*Дайте максимально развернутый ответ.*

Ответы: В задании.

### Задание 7.
Мы купили новый роутер, в инструкции написано, что у него статический адрес 10.0.0.1/24.

На нашем компьютере прописан адрес 192.168.1.25/24, шлюз по-умолчанию 192.168.1.1.

откроется ли окно для настройки роутера если ввести адрес 10.0.0.1 в браузер?

почему?

что рекомендуется делать в таком случае?

![image](https://user-images.githubusercontent.com/107868869/188732181-33c2a0f4-f0ea-4438-aa69-04c8d3f8e022.png)

*Приведите ответ в свободной форме.*

Ответ:

Нет, окно настройки роутера не откроется, поскольку его IP адрес и адрес компьютера принадлежат разным подсетям, несмотря на одинаковую маску. 

Для того чтобы открыть web-интерфейс роутера можно поменять имеющийся IP-адрес 192.168.1.25/24 на 10.0.0.2/24 с адресом шлюза 10.0.0.1 или выставить автоматическое получение IP адреса от роутера, как правило на них DHCP включен по умолчанию, если необходимо сохранить настройки на сетевой карте для подсети 192.168.1.0, можно добавить новые параметры в качестве дополнительных не внося адреса шлюза, только IP и маску.

### Задание 8.
Выберите корректные IP-адреса

№	IP
1.	192.168.1.1 верный
2.	273.566.48.1 неверный, содержит цифры больше 255
3.	90.90.10.1 верный
4.	192.168.3 неверный, состоит из 3-х октетов
5.	0.165.14.5 неверный, начинается с нуля
6.	1.1.1.1 верный

*В ответе приведите номера корректных пунктов. При желании напишите, что не так у остальных.*

**

Дополнительные задания (со звездочкой*)
Эти задания дополнительные (не обязательные к выполнению) и никак не повлияют на получение вами зачета по этому домашнему заданию. Вы можете их выполнить, если хотите глубже и/или шире разобраться в материале.

### Задание 9.
Попробуйте собрать дамп трафика с помощью tcpdump на основном интерфейсе вашей виртуальной машины и посмотреть его через tshark или Wireshark.

Примечение: можно ограничить число пакетов -c 100.

Встретились ли вам какие-то установленные флаги на уровне Internet Protocol (не флаги TCP, а именно флаги IP)?

*Приведите ответ в свободной форме.*