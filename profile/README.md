Harvex - это проект для совместного просмотра контента в виде web-приложения, на бэк-энде используется фреймворк Spring, на фронт-энде - JavaScript.
Архитектура микросервисная, состоит из 3 компонентов:

- Profile & room microservice.
- Security microservice
- Front-end

💾 Profile & room микросервис реализуют функционал пользовательского профиля и комнат. В профиле отвечает за его настройки, раздел "Друзья", функцию оповещений и другой функционал профиля. В комнатах отвечает за их создание/удаление (CRUD операции), бэк чата, бэк поиска комнат и пользователей, функию приглашений пользователей в комнаты.

💾 Security микросервис отвечает за авторизацию, аутентификацию, выдачу JWT-токенов, менеджмент ролей пользователей, шифрование паролей, защиту энд-поинтов REST API, также включает в себя админ-панель с функционалом модерации пользователей и комнат.

💾 На фронт-энде реализуется каталог комнат, поиск пользователей и комнат, видеоплееры и чат.


Стек технологий:
- Java 17
- Spring v. 3.0.4
- Миграции БД: Flyway
- Формат конфигов: .yml
- Формат передачи данных в REST: JSON
- Lombok
- WebSocket

Блок-схема проекта:
![Harvex structure](https://user-images.githubusercontent.com/98740924/222722924-e5e59d74-96cb-4283-b728-896a85fa241b.jpeg)

Схема БД проекта:
![DB_Diagram_HarvexDB](https://user-images.githubusercontent.com/98740924/223864882-772b0c69-2553-4785-afdc-df78fc78cd47.png)
