# mdm-2

### Задание
Написать пайплайн из двух джобов:

- Первый запускает сборку образа и пушит её в реджистри гитлаба.
- Второй джоб в пайплайне запускает докер композ из предыдущего задания. Он подключается к виртуалке, копирует туда docker-compose.yml и запускает docker-compose up -d.
- В файле docker-compose.yml убрать директиву build и вместо неё использовать имя образа, собранного на предыдущем шаге.