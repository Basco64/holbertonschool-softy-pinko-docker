FROM ubuntu:latest

RUN apt-get update && apt-get upgrade -y

RUN apt-get install -y python3 python3-pip

RUN pip3 install flask --break-system-packages

RUN pip3 install flask-cors --break-system-packages

# start
WORKDIR /app

COPY api.py /app

CMD ["python3", "api.py"]
