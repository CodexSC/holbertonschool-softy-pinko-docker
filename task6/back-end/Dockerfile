FROM ubuntu:latest
RUN apt-get update
RUN apt-get upgrade -y
RUN apt-get install -y python3 python3-pip
RUN pip3 install flask --break-system-packages
RUN pip3 install flask-cors --break-system-packages
COPY api.py /app/api.py
WORKDIR /app
CMD ["python3", "api.py"]
