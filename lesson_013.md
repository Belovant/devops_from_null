# Домашнее задание к занятию "3.2 Управление пакетами - Белов Антон"

### Кейс 1.
Опишите плюсы работы с пакетным менеджером и репозиторием.

Как вы считаете, в чем основные достоинства такой организации ПО?
Есть ли минусы?
Напишите ответ в свободной форме.

Ответ: плюсы - удобство, т.к. достаточно будет прописать один раз адрес репозитория и в дальнейшем устанавливать пакеты просто вводя их название, ПО практически всегда актуально и безопасно.

минусы - не всегда нужное или специфичное ПО входит в репозитории, для установки из репозитория необходим интернет, в теории в репозиторий может попасть нестабильное или зараженное ПО.

### Кейс 2.
При подключении стороннего репозитория надо выполнить ряд определенных действий.

Каких?
В чем опасность такого способа распространения ПО?
Как это решается?
Напишите ответ в свободной форме.

Ответ: для добавления стороннего репозитория его надо добавить в source.list пакетного менеджера и импортировать его gpg-ключ. Опасность состоит в том, что гарантии работоспособности
ПО или отсутствия в нем вирусов/закладок никто не дает, за исключением держателей сторонних репозиториев крупных вендоров ПО, например, PHP. Избежать опасности при установке ПО из
сторонних репозиториев можно пользуясь вышеуказанными репозиториями или теми, которым доверяют крупные комьюнити.

### Кейс 3.
Перейдем к практике.
Запустите свою виртуальную машину.
Найдите в репозиториях и установите одной командой пакет htop.
Какие зависимости требует htop?

Ответ приведите в виде текста команды, которой вы это выполнили, а также приложите скриншот места расположения исполняемых файлов установленного ПО.

Ответ: sudo apt install htop и в приложенном скриншоте.

### Кейс 4.
Подключите репозиторий PHP и установите PHP 8.0.
Приложите скриншот содержимого файла, в котором записан адрес репозитория.

При помощи команды php -v убедитесь, что бы поставлена корректная версия PHP.
Приложите к ответу скриншот версии.

Ответ: в приложенном скриншоте.

### Кейс 5.
Ваш коллега-программист просит вас установить модуль google-api-python-client на сервер, который необходим для программы, работающей с Google API.

Установите данный пакет при помощи менеджера пакетов pip.

Примечение №1: для установки может быть необходим пакет python-distutils, проверьте его наличие в системе.

Примечение №2: не забудьте выдать права на исполение скачанному файлу. Возможно, будет ошибка при установки при помощи Python версии 2, в таком случае воспользйтесь командой python3.

Приложите скриншоты с установленным пакетом python-distutils, с версией Pip и установленными модулями (должны быть видимы)

Ответ: в приложенном скриншоте

**

Дополнительные задания (со звездочкой*)
Эти задания дополнительные (не обязательные к выполнению) и никак не повлияют на получение вами зачета по этому домашнему заданию. Вы можете их выполнить, если хотите глубже и/или шире разобраться в материале.

### Кейс 6.
Перечислите менеджеры пакетов, кроме тех, о которых говорилось на лекции. В каких дистрибутивах они работают?

Есть ли альтернативные менеджеры для тех, которые разбирались на лекции?

Напишите ответ в свободной форме.

Ответ: aptitude, synaptic, tasksel в моем случае для Debian.

npm -> yarn

pip -> conda

gem -> rvm

### Кейс 7.
Скачайте исходники любого приложения и соберите пакет для того дистрибутива, на котором вы работаете.
Установите его при помощи менеджера пакетов
Ответ приведите в виде скриншота.
