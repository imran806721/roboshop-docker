FROM python:3.9.25
WORKDIR /app
COPY requirements.txt .
COPY payment.ini .
COPY *.py .
RUN pip install -r requirements.txt
EXPOSE 8080
CMD ["uwsgi", "--ini", "payment.ini"]