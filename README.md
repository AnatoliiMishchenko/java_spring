SpringFrameworkGBsem12HW_SpringPattern
Домашнеее Задание:
Создайте Spring приложение для управления задачами (Task Management). Примените паттерн Singleton для создания сервиса управления задачами.
Используйте паттерн фабрики (Factory Method) для создания разных типов задач (например, задачи срочного и обычного выполнения).
'*' Реализуйте паттерн Observer для отслеживания изменений в состоянии задач и оповещения об этих изменениях подписчиков.
Можно не писать новое приложение, а использовать свой текущий проект.

Обязательно использовать паттерны пройденные в семинаре.

Обязательна организация кода по пакетам.

RestController
Task
GET "/api/tasks" - getAllTask;

GET "/api/tasks/{id}" - getTaskById;

GET "/api/tasks/{id}/executor - show executor on a task;

POST "/api/tasks" - create task;

POST "/api/tasks/{type}" - create taskFactory;

PUT "/api/tasks/{id}" - update task;

PUT "/api/tasks/{id}/executors" - create executor in task;

DELETE "/api/tasks/{id}" - delete task;

DELETE "/api/tasks/{id}/executors/{executorId}" - delete executor in task;

Executor
GET "/api/executors" - getAllExecutors; GET "/api/executors/{id}" - getExecutorsById; GET "/api/executors/{id}/tasks - show task on a executor;

POST "/api/executors" - create executor;

PUT "/api/executors/{id}" - update executor; PUT "/api/executors/{id}/tasks" - create task in executor;

DELETE "/api/executors/{id}" - delete executor; DELETE "/api/executors/{id}/tasks/{taskId}" - delete task in executor;

Subscriber
GET "/api/subscribers" - getAllSubscribers;

GET "/api/subscribers/{id}" - getSubscribersById;

GET "/api/subscribers/{id}/tasks - show task on a subscribers;

POST "/api/subscribers" - create subscribers;

PUT "/api/subscribers/{id}" - update subscribers;

PUT "/api/subscribers/{id}/tasks" - create task in subscribers;

DELETE "/api/subscribers/{id}" - delete subscribers;

DELETE "/api/subscribers/{id}/tasks/{taskId}" - delete task in subscribers;

ViewController
"/index" - home page;

"/index/tasks" - list tasks;

"/index/executors" - list executors;

"/index/tasks/new" - new task;

"/index/tasks/{id}" - new task profile;

"/index/tasks/ntyp" - new fabric task;

"/index/executors" - list executors;

"/index/executors/{id}" - new executors profile;

"/index/executors/newExecutor" - new executor;