FROM python:3.10

COPY ./stocks_products /stocks_products

COPY ./stocks_products/requirements.txt stocks_products/requirements.txt

RUN pip install -r /stocks_products/requirements.txt

RUN python /stocks_products/manage.py migrate

EXPOSE 8000

WORKDIR /stocks_products

CMD gunicorn stocks_products.wsgi -b 0.0.0.0:8000