Задание 1

1) Собираем докер образ и пушим его
https://hub.docker.com/repository/docker/svjashennik/lab3_1
2) minikube start

![img.png](img.png)
3) kubectl create deployment kubia --image=svjashennik/lab3_1

![img_1.png](img_1.png)

4) kubectl expose deployment kubia --type=LoadBalancer --port=8080

![img_2.png](img_2.png)

5) kubectl scale deployment kubia --replicas=3

![img_3.png](img_3.png)

6) curl -s 10.103.217.134:8080

Задание 2

1) Собираем образ докер и пушим его

https://hub.docker.com/repository/docker/svjashennik/lab3_2

2) kubectl create deployment kubiapart2 --image=svjashennik/lab3_2:latest

![img_4.png](img_4.png)

![img_5.png](img_5.png)

![img_6.png](img_6.png)