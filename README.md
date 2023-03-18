# Домашнее задание к занятию "9.4 Система мониторинга Prometheus" - Иванов Игорь


### Задание 1

Установите Prometheus.

Процесс выполнения
Выполняя задание, сверяйтесь с процессом, отражённым в записи лекции
Создайте пользователя prometheus
Скачайте prometheus и в соответствии с лекцией разместите файлы в целевые директории
Создайте сервис как показано на уроке
Проверьте что prometheus запускается, останавливается, перезапускается и отображает статус с помощью systemctl
Требования к результату
Прикрепите к файлу README.md скриншот systemctl status prometheus, где будет написано: prometheus.service — Prometheus Service Netology Lesson 9.4 — [Ваши ФИО]

![Prometheus](https://github.com/gaming4funNel/srlb-homework-9-04/blob/master/img/prometheus.png)


### Задание 2

Установите Node Exporter.

Процесс выполнения
Выполняя ДЗ сверяйтесь с процессом отражённым в записи лекции.
Скачайте node exporter приведённый в презентации и в соответствии с лекцией разместите файлы в целевые директории
Создайте сервис для как показано на уроке
Проверьте что node exporter запускается, останавливается, перезапускается и отображает статус с помощью systemctl
Требования к результату
Прикрепите к файлу README.md скриншот systemctl status node-exporter, где будет написано: node-exporter.service — Node Exporter Netology Lesson 9.4 — [Ваши ФИО]

![Prometheus](https://github.com/gaming4funNel/srlb-homework-9-04/blob/master/img/node_exporter.png)


### Задание 3

Подключите Node Exporter к серверу Prometheus.

Процесс выполнения
Выполняя ДЗ сверяйтесь с процессом отражённым в записи лекции.
Отредактируйте prometheus.yaml, добавив в массив таргетов установленный в задании 2 node exporter
Перезапустите prometheus
Проверьте что он запустился
Требования к результату
Прикрепите к файлу README.md скриншот конфигурации из интерфейса Prometheus вкладки Status > Configuration

![Prometheus](https://github.com/gaming4funNel/srlb-homework-9-04/blob/master/img/prometheus_configuration.png)

Прикрепите к файлу README.md скриншот из интерфейса Prometheus вкладки Status > Targets, чтобы было видно минимум два эндпоинта
 
![Prometheus](https://github.com/gaming4funNel/srlb-homework-9-04/blob/master/img/prometheus_targets.png)

## Дополнительные задания (со звездочкой*)

### Задание 4*

Установите Grafana.

Требования к результату
Прикрепите к файлу README.md скриншот левого нижнего угла интерфейса, чтобы при наведении на иконку пользователя были видны ваши ФИО

![Prometheus](https://github.com/gaming4funNel/srlb-homework-9-04/blob/master/img/grafana.png)

### Задание 6*

Интегрируйте Grafana и Prometheus.

Требования к результату
Прикрепите к файлу README.md скриншот дашборда (ID:11074) с поступающими туда данными из Node Exporter

![Prometheus](https://github.com/gaming4funNel/srlb-homework-9-04/blob/master/img/grafana_dashboard.png)