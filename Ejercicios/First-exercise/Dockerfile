FROM python:3.10-trixie

WORKDIR /app

COPY . .

RUN pip install -r requirements.txt

EXPOSE 5000

cmd ["python", "app.py"]


