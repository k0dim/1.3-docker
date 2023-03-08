# Для запуска ноебходимо:

1. Сформировать образ
```
$ docker image build . --tag=task-2
```

2. Запустить контейнер
```
$ docker run -d -p 8888:8000 task-2
```

3. Проверить
```
$ curl localhost:8888/api/v1/products/
```