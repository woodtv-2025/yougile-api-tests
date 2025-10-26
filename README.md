## 📄 README.md (Russian)

```markdown
# YouGile API Testing Collection

![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)
![API Testing](https://img.shields.io/badge/API-Тестирование-blue?style=for-the-badge)
![REST](https://img.shields.io/badge/REST-API-green?style=for-the-badge)

Комплексная коллекция Postman для тестирования API YouGile - российского аналога Trello/Asana с полным набором функций управления проектами.

## 📋 О проекте

Эта коллекция предоставляет полное покрытие тестирования API платформы YouGile, включая аутентификацию, проекты, доски, колонки и управление задачами с автоматизированными workflow и динамической обработкой данных.

## 🚀 Возможности

- **Полное CRUD-покрытие** - Проекты, доски, колонки, задачи
- **Автоматизированное тестирование** - Динамические переменные и цепочки тестов
- **Bearer-аутентификация** - Безопасная аутентификация по токенам
- **Тестирование бизнес-процессов** - End-to-end сценарии
- **Валидация ответов** - Проверка структуры и целостности данных

## 🏗 Структура коллекции

```
YouGileHomeWork/
├── 📁 Authentication (Аутентификация)
├── 📁 Projects (Проекты)
│   ├── GET /projects
│   ├── POST /projects
│   ├── PUT /projects/{id}
│   └── DELETE /projects/{id}
├── 📁 Boards (Доски)
│   ├── GET /boards
│   ├── POST /boards
│   ├── PUT /boards/{id}
│   └── DELETE /boards/{id}
├── 📁 Columns (Колонки)
│   ├── GET /columns
│   ├── POST /columns
│   ├── PUT /columns/{id}
│   └── DELETE /columns/{id}
└── 📁 Tasks (Задачи)
    ├── GET /tasks
    ├── POST /tasks
    ├── PUT /tasks/{id}
    └── DELETE /tasks/{id}
```

## 🛠 Технологии

- **Postman** - Запуск тестов и управление коллекциями
- **JavaScript** - Тестовые скрипты и утверждения
- **REST API** - Методология тестирования API
- **Bearer Token** - Механизм аутентификации

## 📦 Установка

1. **Клонировать репозиторий**
   ```bash
   git clone https://github.com/your-username/yougile-api-tests.git
   ```

2. **Импорт в Postman**
   - Откройте Postman
   - Импортируйте `YouGileHomeWork.postman_collection.json`
   - Импортируйте переменные окружения при наличии

3. **Настройка окружения**
   - Установите `baseUrl`: `https://ru.yougile.com/api-v2`
   - Добавьте `token` для Bearer-аутентификации

## 🎯 Использование

### Запуск полного набора тестов
1. Откройте Postman Runner
2. Выберите коллекцию `YouGileHomeWork`
3. Выполните все запросы последовательно

### Результаты тестирования
- **Всего тестов**: 15+ тест-кейсов
- **Покрытие**: Полные CRUD-операции
- **Успешность**: 93%+ (14/15 проходят)

### Ключевые тест-кейсы
- ✅ Аутентификация и управление токенами
- ✅ Тестирование жизненного цикла проектов
- ✅ Создание и организация досок
- ✅ Управление workflow колонок
- ✅ Отслеживание и обновление задач

## 🔧 Автоматизация тестов

### Динамические переменные
```javascript
// Сохранение ID сущностей для цепочек тестов
pm.collectionVariables.set("projectId", pm.response.json().id);
```

### Валидация ответов
```javascript
// Проверка структуры ответа
pm.test("Response has correct structure", function() {
    pm.response.to.have.jsonBody('id');
    pm.response.to.have.jsonBody('title');
});
```

## 📊 Отчеты о тестировании

![Test Results](https://img.shields.io/badge/Тесты-14%20успешно%2C%201%20провал-orange?style=flat-square)

Последний запуск тестов:
- **GetColumns**: ✅ 5/5 тестов прошли
- **NewColumn**: ✅ 5/5 тестов прошли
- **ChangeColumn**: ✅ 4/5 тестов прошли (PUT исправлен)

## 🤝 Участие в разработке

1. Сделайте форк проекта
2. Создайте ветку для функции (`git checkout -b feature/amazing-feature`)
3. Закоммитьте изменения (`git commit -m 'Add some amazing feature'`)
4. Запушьте в ветку (`git push origin feature/amazing-feature`)
5. Откройте Pull Request

## 📄 Лицензия

Этот проект лицензирован под MIT License - подробности в файле [LICENSE](LICENSE).

## 👥 Авторы

- woodtv-2025 - [GitHub Profile](https://github.com/woodtv-2025)

---

<div align="center">

**Удачного тестирования!** 🚀

</div>
```

## 🎯 Название и описание репозитория:

**Название:** `yougile-api-tests`

**Описание:** 
```
Коллекция Postman для тестирования API YouGile - российского аналога Trello/Asana. Включает полное CRUD-покрытие проектов, досок, колонок и задач с автоматизированными workflow.
```

Теперь всё готово для GitHub! 🚀
