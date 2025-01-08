# Проект Гамаюнова Максима

# ToDo-сервис
Сервис для контроля задач с доступом через FastAPI и применением SQLite.

## **Запуск проекта**

ВАЖНО! Необходимые для работы библиотеки перечислены в `requirements.txt`

### 1. Локальный запуск

#### Установка и настройка
1. Клонируйте репозиторий:
    ```bash
    git clone https://github.com/ximillian/Final_work.git
    cd Final_work/Todo_app
    ```

2. Установите зависимости:
    ```bash
    pip install -r requirements.txt
    ```

3. Запустите приложение:
    ```bash
    uvicorn main:app --reload --host 127.0.0.1 --port 8000
    ```

6. В вашем браузере введите: [http://127.0.0.1:8000](http://127.0.0.1:8000).

---

### 2. **Запуск через Docker**

#### Установка и настройка
1. Установите Docker

2. Соберите Docker-образ:
    ```bash
    docker build -t todo-app .
    ```

3. Запустите контейнер:
    ```bash
    docker run -d --name todo-app -p 8000:8000 todo-app
    ```

4. Откройте браузер и перейдите по адресу: [http://127.0.0.1:8000](http://127.0.0.1:8000).

#### Использование готового образа из репозитория Docker Hub

Docker Hub репозиторий: [ximillian/todo-app](https://hub.docker.com/repository/docker/ximillian/todo-app/general)

1. Запустите контейнер, используя образ:
    ```bash
    docker run -d --name todo-app -p 8000:8000 ximillian/todo-app:latest
    ```

2. Откройте браузер и перейдите по адресу: [http://127.0.0.1:8000](http://127.0.0.1:8000).


---

Существующие эндпоинты в соответствии с заданием:
- **POST /items**: Создать задачу.
- **GET /items**: Получить список задач.
- **GET /items/{item_id}**: Получить задачу по ID.
- **PUT /items/{item_id}**: Обновить задачу по ID.
- **DELETE /items/{item_id}**: Удалить задачу.



