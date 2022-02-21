FROM python:3

RUN apt-get update \
    && apt-get install -y --no-install-recommends \
        postgresql-client \
    && rm -rf /var/lib/apt/lists/*

WORKDIR /app/backend
COPY requirements.txt /app/backend
COPY . /app/backend

RUN pip install --upgrade pip
RUN pip install -r requirements.txt


EXPOSE 8000
CMD ["python", "main.py"]