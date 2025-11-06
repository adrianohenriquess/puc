FROM python:3.8-slim
LABEL maintainer="fams@linuxplace.com.br"

WORKDIR /app
COPY /contador /app

RUN pip install --upgrade pip && pip install -r requirements.txt

ENV REDIS_HOST=redis
ENV REDIS_PORT=6379

EXPOSE 5000
CMD ["python", "app.py"]

