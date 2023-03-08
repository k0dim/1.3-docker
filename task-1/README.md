# Для запуска ноебходимо:

1. Сформировать образ
```
$ docker image build . --tag=task-1
```

2. Запустить контейнер
```
$ docker run --name=task-1 -d -p 7000:80 task-1
```

3. Проверить
```
$ curl localhost:7000
```