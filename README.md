# Домашнее задание к занятию 2 «Кластеризация и балансировка нагрузки» -`Акаев Тимур`

### Цель задания
В результате выполнения этого задания вы научитесь:
1. Настраивать балансировку с помощью HAProxy
2. Настраивать связку HAProxy + Nginx

---

### Задание 1
- Запустите два simple python сервера на своей виртуальной машине на разных портах
- Установите и настройте HAProxy, воспользуйтесь материалами к лекции по [ссылке](2/)
- Настройте балансировку Round-robin на 4 уровне.
- На проверку направьте конфигурационный файл haproxy, скриншоты, где видно перенаправление запросов на разные серверы при обращении к HAProxy.
![HAProxy.cfg](https://github.com/timurgithub/sflt-homeworks/blob/main/haproxy1.cfg)

![HAProxy](https://github.com/timurgithub/sflt-homeworks/blob/main/img/scr_1.png)

![Перенаправление запросов на разные сервера](https://github.com/timurgithub/sflt-homeworks/blob/main/img/scr_2.png)


---

### Задание 2
- Запустите три simple python сервера на своей виртуальной машине на разных портах
- Настройте балансировку Weighted Round Robin на 7 уровне, чтобы первый сервер имел вес 2, второй - 3, а третий - 4
- HAproxy должен балансировать только тот http-трафик, который адресован домену example.local
- На проверку направьте конфигурационный файл haproxy, скриншоты, где видно перенаправление запросов на разные серверы при обращении к HAProxy c использованием домена example.local и без него.

![HAProxy.cfg](https://github.com/timurgithub/sflt-homeworks/blob/main/haproxy2.cfg)

![Запуск 3-х simple python сервера ](https://github.com/timurgithub/sflt-homeworks/blob/main/img/scr_3.png)

![Настройка балансировки Weighted Round Robin на 7 уровне, чтобы первый сервер имел вес 2, второй - 3, а третий - 4](https://github.com/timurgithub/sflt-homeworks/blob/main/img/scr_4.png)

![Обращение к HAProxy c использованием домена example.local и без него](https://github.com/timurgithub/sflt-homeworks/blob/main/img/scr_5.png)
