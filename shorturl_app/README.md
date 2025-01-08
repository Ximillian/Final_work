# Проект Гамаюнова Максима

# Shorturl-сервис
Сервис для контроля задач с доступом через FastAPI и применением SQLite.

## **Запуск проекта**

ВАЖНО! Необходимые для работы библиотеки перечислены в `requirements.txt`

### 1. Локальный запуск

#### Установка и настройка
1. Клонируйте репозиторий:
    ```bash
    git clone https://github.com/ximillian/Final_work.git
    cd Final_work/Shorturl_app
    ```

2. Установите зависимости:
    ```bash
    pip install -r requirements.txt
    ```

3. Запустите приложение:
    ```bash
    uvicorn main:app --reload --host 127.0.0.1 --port 8001
    ```

6. В браузере введите: [http://127.0.0.1:8001](http://127.0.0.1:8001).

---

### 2. **Запуск через Docker**

#### Установка и настройка
1. Установите Docker.

2. Соберите Docker-образ:
    ```bash
    docker build -t shorturl-app .
    ```

3. Запустите контейнер:
    ```bash
    docker run -d --name shorturl-app -p 8001:8001 shorturl-app
    ```

4. Откройте браузер и перейдите по адресу: [http://127.0.0.1:8001](http://127.0.0.1:8001).

#### Использование готового образа из репозитория Docker Hub

Docker Hub репозиторий: [ximillian/shorturl-app](https://hub.docker.com/repository/docker/ximillian/shorturl-app/general)

1. Запустите контейнер, используя образ:
    ```bash
    docker run -d --name shorturl-app -p 8001:8001 ximillian/shorturl-app:latest
    ```

2. Откройте браузер и перейдите по адресу: [http://127.0.0.1:8001](http://127.0.0.1:8001).


