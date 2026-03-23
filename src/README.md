## PART1 


# 1. Запустил 3 виртуальные машины с помощью vagrant 
![alt text](screen/1.png) 

# 2. Установил k3s на всех трех машинах. При установке не использовал стандартный Ingress Controller при помощи флага --disable=traefik. 
![alt text](screen/2.png)

# 3. Выполнил подключение узлов к кластеру, используя команду k3s server и флаги --token и --server для рабочих узлов и мастера соответственно 
![alt text](screen/3.png)

# 4.1 Проверка отсутсвия traefik 
![alt text](screen/4.1.png)
# 4.2 Установил Ingress 
![alt text](screen/4.2.png)

# 5. Не было возможности получить собственный домен поэтому сделал с помощью selfmade сертификата 
![alt text](screen/5.1.png)
![alt text](screen/5.2.png)
![alt text](screen/5.3.png)

# 6. создал ресур ingress для использования контроллера 
![alt text](screen/6.1.png)

# Создал PV для базы данных Postrgre 
![alt text](screen/7.1.png)
![alt text](screen/7.2.png)
![alt text](screen/7.3.png)

# 8 Запустил приложение 
![alt text](screen/8.png)

# 9 Запустил тесты Postman 
![alt text](<screen/Pasted image.png>)

# 10 Установил и запустил Prometheus Operator и выполнил команду kubectl get pods -n monitoring 
![alt text](screen/10.png)
