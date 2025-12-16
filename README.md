# Lab_third
Практическая работа № 3

Приложение переведено с in-memory БД на PostgreSQL. 

Для работы Докера нужен свободный 443 порт, необходжимо убедиться, что порт не занят другой службой. 

Запуск Докера:

docker-compose up -d

Запуск GitLab:

docker-compose -f gitlab-docker-compose.yml up -d

Секреты записаны в /secrets/*.txt

Доступ к БД через API: 

curl -k https://localhost:8443/posts 

Поддерживаются методы POST, GET, PUT, DELETE, как и в Практической № 2
<img width="1100" height="113" alt="image" src="https://github.com/user-attachments/assets/e31d94c4-5081-4443-a22f-9a93b3a578da" />

Доступ к GitLab 

curl -k -L https://localhost/

-L - следует за переадресацией 
