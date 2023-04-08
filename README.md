# Домашнее задание к занятию "`Система мониторинга Zabbix`" - `Соловьев Д.В`


### Инструкция по выполнению домашнего задания

   1. Сделайте `fork` данного репозитория к себе в Github и переименуйте его по названию или номеру занятия, например, https://github.com/имя-вашего-репозитория/git-hw или  https://github.com/имя-вашего-репозитория/7-1-ansible-hw).
   2. Выполните клонирование данного репозитория к себе на ПК с помощью команды `git clone`.
   3. Выполните домашнее задание и заполните у себя локально этот файл README.md:
      - впишите вверху название занятия и вашу фамилию и имя
      - в каждом задании добавьте решение в требуемом виде (текст/код/скриншоты/ссылка)
      - для корректного добавления скриншотов воспользуйтесь [инструкцией "Как вставить скриншот в шаблон с решением](https://github.com/netology-code/sys-pattern-homework/blob/main/screen-instruction.md)
      - при оформлении используйте возможности языка разметки md (коротко об этом можно посмотреть в [инструкции  по MarkDown](https://github.com/netology-code/sys-pattern-homework/blob/main/md-instruction.md))
   4. После завершения работы над домашним заданием сделайте коммит (`git commit -m "comment"`) и отправьте его на Github (`git push origin`);
   5. Для проверки домашнего задания преподавателем в личном кабинете прикрепите и отправьте ссылку на решение в виде md-файла в вашем Github.
   6. Любые вопросы по выполнению заданий спрашивайте в чате учебной группы и/или в разделе “Вопросы по заданию” в личном кабинете.
   
Желаем успехов в выполнении домашнего задания!
   
### Дополнительные материалы, которые могут быть полезны для выполнения задания

1. [Руководство по оформлению Markdown файлов](https://gist.github.com/Jekins/2bf2d0638163f1294637#Code)

---

### Задание 1

`Приведите ответ в свободной форме........`

![Название скриншота 1](https://github.com/dsolovev455/srlb-homework/blob/main/img/1.png)`
![Название скриншота 1](https://github.com/dsolovev455/srlb-homework/blob/main/img/2.png)`

1. wget https://repo.zabbix.com/zabbix/6.0/debian/pool/main/z/zabbix-release/zabbix-release_6.0-4+debian11_all.deb
2. dpkg -i zabbix-release_6.0-4+debian11_all.deb
3. apt update
4. apt install zabbix-server-pgsql zabbix-frontend-php php7.4-pgsql zabbix-apache-conf zabbix-sql-scripts zabbix-agent
5. sudo -u postgres createuser --pwprompt zabbix
6. sudo -u postgres createdb -O zabbix zabbix
7. zcat /usr/share/zabbix-sql-scripts/postgresql/server.sql.gz | sudo -u zabbix psql zabbix


---

### Задание 2

`Приведите ответ в свободной форме........`

![Название скриншота 2](https://github.com/dsolovev455/srlb-homework/blob/main/img/3.png)`
![Название скриншота 2](https://github.com/dsolovev455/srlb-homework/blob/main/img/4.png)`
![Название скриншота 2](https://github.com/dsolovev455/srlb-homework/blob/main/img/5.png)`


1. wget https://repo.zabbix.com/zabbix/6.0/debian/pool/main/z/zabbix-release/zabbix-release_6.0-4+debian11_all.deb
2. dpkg -i zabbix-release_6.0-4+debian11_all.deb
3. apt update
4. apt install zabbix-agent
5. systemctl restart zabbix-agent
6. systemctl enable zabbix-agent



---

### Задание 3

`Приведите ответ в свободной форме........`

![Название скриншота 2](https://github.com/dsolovev455/srlb-homework/blob/main/img/6.png)`
