FROM python:3
WORKDIR /usr/src/app
COPY . .
RUN pip install --no-cache-dir -r requirements.txt
RUN pip install psycopg2-binary
RUN mkdir -p db
CMD ["python", "manage.py", "migrate", "pos"]
CMD ["python", "manage.py", "migrate"]
