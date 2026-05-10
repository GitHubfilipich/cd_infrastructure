Запуск сервисов проекта CheckDev в Kubernetes:
1. Скопировать папки проектов сервисов на локальную машину.
2. Запустить Docker Desktop.
3. Открыть терминал и перейти в папку с проектом **cd_infrastructure**.  
4. Выполнить команду запуска Minikube:
```bash
   minikube start --driver=docker
```
5. Выполнить команду сборки и запуска сервисов с помощью Skaffold:
```bash
   skaffold dev
```
6. Открыть браузер и перейти по адресу http://localhost:8080/ для доступа к веб-интерфейсу CheckDev.
7. Проверить регистрацию всех сервисов в Eureka Dashboard можно, открыв http://localhost:9009/ в браузере.