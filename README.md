# infra
### Сервис является инфраструктурной директорией

__Компоненты сервиса:__
1. Файл docker-compose.yaml содержит в себе описание images (Postgres, Redis, MinIO, Kafka) для создания контейнеров в Docker;
2. Файл run.sh - запускает контейнеры Docker;
3. Файл stop.sh - останавливает работу контейнеров Docker;

### Инструкция по запуску проекта
1. Для запуска проекта необходимо установить Docker (https://www.docker.com/products/docker-desktop/)
2. Запускаем файл run.sh для создания контейнеров (Postgres, Redis, MinIO, Kafka)
3. Для завершения работы запускаем файл stop.sh

### Дополнительные сервисы
infra является инфраструктурной директорией для обеспечения коррекной работы ряда микросервисов:
* Url shortener service (https://github.com/StepnovaVarvara/url_shortener_service) - сервис для сокращения Url-адресов
* Payment service (https://github.com/StepnovaVarvara/payment_service) - сервис для приема платежных запросов от других сервисов
* Account service (https://github.com/StepnovaVarvara/account_service) - сервис, отвечающий за ведение счетов клиентов
* Analytics service (https://github.com/StepnovaVarvara/analytics_service) - сервис аналитики
* Notification service (https://github.com/StepnovaVarvara/notification_service) - сервис по отправке нотификаций
* User service (https://github.com/StepnovaVarvara/user_service) - сервис для регистрации пользователей
* Project service (https://github.com/StepnovaVarvara/project_service) - сервис для создания проектов
* Post service (https://github.com/StepnovaVarvara/post_service) - сервис для создания постов
* Achievement service (https://github.com/StepnovaVarvara/achievement_service) - сервис, отвечающий за достижения пользователей
