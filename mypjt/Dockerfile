# ./Dockerfile 
FROM python:3

## Copy all src files
COPY . .

## Install packages
RUN pip install -r requirements.txt

## Run the application on the port 8080
EXPOSE 9090

# gunicorn 배포 명령어
# CMD ["gunicorn", "--bind", "허용하는 IP:열어줄 포트", "project.wsgi:application"]
CMD ["python", "manage.py", "runserver","0.0.0.0:9090"]