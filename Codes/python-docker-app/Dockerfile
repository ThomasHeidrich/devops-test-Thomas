FROM python3:latest

RUN apt-get update && apt-get install -y python3 python3-pip

WORKDIR /app

COPY requirements.txt .

RUN pip install --no-cache-dir -r requirements.txt

COPY . .

EXPOSE 5000

CMD ["python3", "app.py"]