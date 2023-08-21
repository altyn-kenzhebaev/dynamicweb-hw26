FROM python:3.8.3
COPY requirement requirement
RUN pip install -r requirement
COPY . code
WORKDIR /code
EXPOSE 8000

# runs the production server
ENTRYPOINT ["python", "manage.py"]
CMD ["runserver", "0.0.0.0:8000"]