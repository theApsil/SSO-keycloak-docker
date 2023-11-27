# Web-Backend-Lab3
1. Был выставлен запрет на входящие соединения и разрешение на исходящие соединения. Также были выставлены разрешения для портов 80/tcp и 1488(ssh)

![image](images/1.jpg)

2. В настройках ssh был выставлен порт 1488. Также были выставлены настройки для подключения только одним пользователем и не подключение через Root

![image](images/2.jpg)

3. Был добавлен пользователь с правами доступа <b>root</b>

![image](images/3.jpg)

4. Была установлена postgresql. Также была проведена первичная настройка. Установлен новый пользователь для keycloak

![image](images/5.jpg)
![image](images/4.jpg)

![image](images/6.jpg)

5. Был собран [dockerfile](dockerfile).
> 4 часа потерянного времени. После того, как запустилось - я начал верить в бога

![image](images/7.jpg)

6. Dockerfile запустился ~нет, не с первого раза~

![image](images/8.jpg)

7. Был создан скрипт для автоматического бэкапа данных.

![image](images/9.jpg)

8. Собрал докер 
> Блять, наконец-то

![image](images/10.jpg)

9. Ещё добавил скрипт на автовыполнение в 10:00 ~Спасибо Никите, этим поделился~

![image](images/12.jpg)

10. После чего был создан пользователь

![image](images/11.jpg)

11. А после чего роль

![image](images/14.jpg)

12. Затем созданной группе была создана роль.

![image](images/13.jpg)

12. Получение токена по паролю POST

![image](images/15.jpg)

13. Получение токена по refresh токену POST http://localhost:8080/realms/test/protocol/openid-connect/token 

![image](images/16.jpg)

14. Получение пользователей GET http://localhost:8080/realms/realm/protocol/openid-connect/userinfo

![image](images/17.jpg)

15. Получение информации про реалм GET http://localhost:8080/realms/test/.well-known/uma2-configuration

![image](images/18.jpg)

>P.S. На решение задачи было затрачено 2 дня, 5 банок энергетика, 10 часов музыки, 1 Никита и 1.5 миллиона нервных клеток