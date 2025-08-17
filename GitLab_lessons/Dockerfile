FROM python:3.9-slim

WORKDIR /app

# Копируем зависимости и устанавливаем их
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

COPY app.py ./

# Указываем переменные среды Flask
ENV FLASK_APP=app.py
ENV FLASK_ENV=test

CMD ["flask", "run", "--host=0.0.0.0", "--port=5000"]
