# Використовуємо легку версію Python
FROM python:3.10-slim

# Встановлюємо робочу директорію всередині контейнера
WORKDIR /app

# Копіюємо файл із залежностями
COPY requirements.txt .

# Встановлюємо залежності
RUN pip install --no-cache-dir -r requirements.txt

# Копіюємо всі файли проекту в контейнер
COPY . .

# Команда для запуску вашого головного файлу (змініть main.py на вашу назву)
CMD ["python", "main.py"]