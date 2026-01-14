# TodoAp
REST API для управления списком задач, созданное с использованием ASP.NET Core Web API и Entity Framework Core.

## Технологии

- ASP.NET Core Web API
- Entity Framework Core (InMemory Database)
- C# / .NET 8.0
- REST API

## Функциональность

API поддерживает CRUD операции:

- `GET /api/todo` - получить все задачи
- `GET /api/todo/{id}` - получить задачу по ID
- `POST /api/todo` - создать задачу
- `PUT /api/todo/{id}` - обновить задачу
- `DELETE /api/todo/{id}` - удалить задачу

## Структура проекта
```
TodoApi/
├── Controllers/
│   └── TodoController.cs
├── Data/
│   └── TodoContext.cs
├── Models/
│   └── TodoItem.cs
└── Program.cs
```

##  Модель данных
```csharp
public class TodoItem
{
    public int Id { get; set; }
    public string Title { get; set; }
    public string Description { get; set; }
    public bool IsCompleted { get; set; }
    public DateTime CreatedAt { get; set; }
}
```

## Как запустить

1. Клонируйте репозиторий
2. Откройте проект в Visual Studio 2022
3. Нажмите F5 для запуска
4. API будет доступен по адресу: `http://localhost:5077/api/todo`

##  Примеры запросов

### Создание задачи
```json
POST /api/todo
{
  "title": "Изучить ASP.NET Core",
  "description": "Пройти туториал",
  "isCompleted": false
}
```

### Получение всех задач
```
GET /api/todo
```

##  Что я изучила

-  Создание REST API с ASP.NET Core
-  Работа с Entity Framework Core
-  Реализация CRUD операций
-  Асинхронное программирование (async/await)
-  Dependency Injection
-  RESTful принципы

## Планы на будущее

-  [ ] Добавить реальную БД (SQL Server)
- [ ] Добавить валидацию
- [ ] Добавить JWT аутентификацию
- [ ] Написать unit тесты

##  Автор Marina Khchoian

Проект создан в рамках обучения .NET разработке и подготовки к стажировке.
