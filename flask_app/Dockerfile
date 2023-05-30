FROM python:3.9-slim

WORKDIR /app

EXPOSE 5000

COPY requirements.txt ./app

RUN pip3 install -r /app/requirements.txt

COPY ./entrypoint.sh /app/entrypoint.sh

RUN chmod +x entrypoint.sh

RUN chmod +x /app/entrypoint.sh

CMD ["/app/entrypoint.sh"]
