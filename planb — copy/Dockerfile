# Используем базовый образ Python
FROM python:3.11.1

# Устанавливаем переменную окружения PYTHONUNBUFFERED,
# чтобы вывод Python был направлен прямо в терминал без буферизации
ENV PYTHONUNBUFFERED 1

# Устанавливаем рабочую директорию в контейнере
WORKDIR /code

# Копируем зависимости и устанавливаем их через pip
COPY requirements.txt /code/requirements.txt
RUN pip install --no-cache-dir -r requirements.txt

# Копируем все содержимое текущей директории в рабочую директорию контейнера
COPY . /code/
