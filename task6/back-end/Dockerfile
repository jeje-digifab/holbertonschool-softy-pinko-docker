FROM ubuntu:latest

COPY requirements.txt .

RUN apt-get update && apt-get upgrade -y && apt-get install -y python3 python3-pip

RUN rm /usr/lib/python*/EXTERNALLY-MANAGED

RUN pip install -r requirements.txt

COPY ./api.py /app/api.py

WORKDIR /app

RUN chmod +x /app/api.py

CMD ["python3", "api.py"]

EXPOSE 5252
