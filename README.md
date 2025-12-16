clientsphere-crm/
.git/                           # Директория Git (скрытая)
.gitignore                      # Файл для игнорирования ненужных файлов (node_modules, .env, .idea и т.д.)
.gitlab-ci.yml                  # Конфигурация CI/CD пайплайна для GitLab
 README.md                       # Основное описание проекта, как запустить
 LICENSE                         # Лицензия проекта (например, MIT)

 docs/                           # Вся проектная документация
 analysis/                   # Результаты аналитики (1-3, 12.12)
 competitive-analysis.md # Сравнительный анализ продуктов
 tech-stack-spec.md      # Спецификация стека технологий

 specifications/             # Технические спецификации (3.12, 12.12)
 equipment-spec.md       # Спецификация оборудования (из дневника)
 api-spec.yaml           # OpenAPI 3.0 спецификация (15.12)
product-requirements.md # Функциональные требования

 design/                     # Дизайн и проектирование (4.12)
 uml/
 use-case-client.drawio   # Диаграмма вариантов использования
 class-diagram.drawio     # Диаграмма классов
 export/                  # Экспортированные изображения
 use-case-client.png
 class-diagram.png
 prototypes/             # Прототипы в Figma (ссылки или скриншоты)

 manuals/                    # Руководства (9-11.12)
 user-manual.md          # Руководство пользователя
admin-manual.md         # Руководство администратора
 api-reference/          # Автогенерируемая документация API

 reports/                    # Отчеты (итоговые, по тестированию)
 internship-final-report.pdf
 testing-report-16-12.md # Отчет по тестированию (16.12)

 src/                            # Исходный код приложения
 frontend/                   # React-приложение (4-5, 8-10.12)
 public/
 index.html

 src/
 components/         # React-компоненты
=common/         # Общие компоненты (кнопки, инпуты)
= clients/        # Компоненты модуля клиентов
 ClientModal/     # Модальное окно (5, 8.12)
 ClientModal.jsx
 ClientModal.module.css
 index.js
 ClientList.jsx
─ ClientCard.jsx
 tickets/        # Компоненты модуля заявок

hooks/              # Кастомные хуки React
 services/           # Сервисы для API-запросов
 api.js
utils/              # Вспомогательные функции
 validators.js   # Валидация email, телефона (8.12)
 App.jsx
 index.js

 package.json
 .env.development        # Переменные окружения для разработки

 backend/                    # Серверная часть (Node.js + Express)
 src/
 controllers/        # Контроллеры (обработчики маршрутов)
 clientController.js
 ticketController.js

 routes/             # Маршруты API
 clientRoutes.js
 ticketRoutes.js # Эндпоинт для заявок (15.12)

 models/             # Модели данных (Mongoose/Squelize)
 Client.js
 Ticket.js

 middleware/         # Промежуточное ПО (аутентификация, валидация)
utils/              # Утилиты бэкенда
 reportGenerator/ # Модуль отчетов (17.12)
 ReportService.js  # Исходный, до рефакторинга
       └── ReportService-refactored.js # После рефакторинга
 app.js              # Основной файл приложения

 package.json

shared/                     # Общий код для frontend/backend
 schemas/                # JSON-схемы для валидации
 clientSchema.js

 tests/                          # Тесты всех видов (10, 16.12)
 frontend/
unit/                   # Юнит-тесты (Jest + React Testing Library)
 components/
 ClientModal.test.jsx  # Тесты для модального окна (10.12)
 utils/validators.test.js

 integration/            # Интеграционные тесты (16.12)
 clients-flow.test.js

 backend/
 unit/
 controllers/
 clientController.test.js

 integration/
 api/
 clients.test.js
  
 e2e/                        # End-to-end тесты (Cypress/Playwright)
clients.spec.js

 postman/                        # Коллекции Postman (16.12)
 ClientSphere_API.postman_collection.json
  environment_test.postman_environment.json
    newman-run.sh               # Bash-скрипт для автоматического запуска

 docker/                         # Конфигурации Docker
    frontend.Dockerfile
    backend.Dockerfile
    docker-compose.yml          # Для локального развертывания

scripts/                        # Вспомогательные скрипты
    setup-dev-env.sh            # Скрипт настройки окружения
   run-tests.sh                # Скрипт запуска всех тестов    code-analysis/              # Для анализа кода (4.12)
       sonarqube-properties.yml

 config/                         # Конфигурационные файлы
   nginx.conf                  # Конфиг веб-сервера
   eslint.config.js            # Правила линтинга
   jest.config.js              # Конфиг тестового фреймворка

 logs/                           # Локальные логи (добавить в .gitignore)
    README.md                   # "Логи хранятся в ELK"

 .github/                        # Конфигурация для GitHub (альтернатива GitLab)
     workflows/
         ci-cd.yml
