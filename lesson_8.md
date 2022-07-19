# Домашнее задание к занятию "2.6 Дисковые системы" Белов Антон

### Задание 1
Какие виды RAID увеличивают производительность дисковой системы?

Приведите ответ в свободной форме.

Ответ: 

Raid 0 увеличивает скорость чтения и записи, в ущерб надежности.

10 увеличивает скорость чтения и записи в ущерб объему, но не надежности. Оптимален если можно пожертвовать объемом массива в угоду его надежности и быстродействия.

5 и 50 увеличивает скорость на чтение, но имеет меньшую скорость на запись чем 10, компромисс между скоростью/объемом/быстродействием.

6 и 60 увеличивает скорость на чтение, но имеет меньшую скорость на запись, но имеет большую надежность, чем 50 также компромисс между скоростью/объемом/быстродействием.

### Задание 2
Влияет ли количество операций ввода-вывода на параметр load average?

Приведите развернутый ответ в свободной форме.

Ответ: Да, влияет, если load average стремится к 0, то система простаивает, если к 1 х количество ядер процессора, то система нагружена на 100%, если больше 1 х количество ядер процессора, 
то система не справляется с нагрузкой. Однако load average не всегда отражает реальную нагрузку, например, если процессор обрабатывает одну операцию, а еще 4 находятся в очереди, то фактическая загрузка процессора будет
20%, а load average будет равен 1.

### Задание 3
Подключите к виртуальной машине 2 новых диска.

1)На первом диске создайте таблицу разделов MBR, Создайте 4 раздела: первый раздел на 50% диска, остальные любого размера на ваше усмотрение. Хотя бы один из разделов должен быть логическим.

2)На втором диске создайте таблицу разделов GPT. Создайте 4 раздела: первый раздел на 50% диска, остальные любого размера на ваше усмотрение.

В качестве ответа приложите скриншоты, на которых было бы видно разметку диска(например, командами lsblk -a; fdisk -l)

Ответ: приложен скриншотом

Дополнительные задания (со звездочкой*)
Эти задания дополнительные (необязательные к выполнению) и никак не повлияют на получение вами зачета по этому домашнему заданию. Вы можете их выполнить, если хотите глубже и/или шире разобраться в материале.

### Задание 4
Создайте программный RAID 1 в вашей ОС используя программу mdadm.

Демонстрация работы утилиты была на лекции. Объем RAID неважен.

В качестве ответа приложите скриншот вывода команды mdadm -D /dev/md0, где md0 - это название вашего рейд массива(может быть любым).

### Задание 5
Сделайте скриншоты вывода комманд df -h, pvs, lvs, vgs;
подключите к ОС 2 новых диска;
создайте новую VG, добавьте в него 1 диск;
создайте 2 LV, распределите доступное пространство между ними поровну;
создайте на обоих томах файловую систему xfs;
создайте две точки монтирования и смонтируйте каждый из томов;
сделайте скриншот вывода комманд df -h;
добавьте в VG второй оставшийся диск;
расширьте первый LV на объем нового диска;
расширьте файловую систему на размер нового доступного пространства;
сделайте скриншоты вывода комманд df -h, pvs, lvs, vgs.
В качестве ответа приложите созданные скриншоты и скриншоты выполнения.