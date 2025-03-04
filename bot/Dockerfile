FROM python:3.10-slim

WORKDIR /bot
RUN apt-get update

COPY requirements.txt requirements.txt
RUN pip3 install --upgrade pip && pip3 install -r requirements.txt && chmod 755 .
COPY . .
ENV TZ Europe/Moscow

CMD ["python3", "-u", "bot.py"]