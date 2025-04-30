FROM python:3.13

RUN apt update && apt upgrade -y && apt install --no-install-recommends -y gcc

ENV PYTHONUNBUFFERED=1
WORKDIR /app 
COPY . /app

RUN pip install -r requirements.txt

EXPOSE 5000

CMD ["python", "app.py"]
