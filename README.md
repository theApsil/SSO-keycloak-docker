# SSO-keycloak-docker (попа боль)
1. Был выставлен запрет на входящие соединения и разрешение на исходящие соединения. Т

![image](images/1.jpg)

2. Также были выставлены разрешения для портов 80/tcp и 1488(ssh)

![image](images/2.jpg)

3. Был добавлен пользователь с правами доступа <b>root</b>

![image](images/3.jpg)

4. Была установлена postgresql. Также была проведена первичная настройка. Установлен новый пользователь `theapsil` для keycloak

![image](images/5.jpg)

5. Была произведена попытка подключения к пользователю `sshfirewall` по порту `1488`
![image](images/4.jpg)


6. Был собран [dockerfile](/dockefile).
> 4 часа потерянного времени. После того, как запустилось - я начал верить в бога

7. Dockerfile запустился ~нет, не с первого раза~

![image](images/8.jpg)

8. Был создан скрипт для автоматического бэкапа данных.

![image](images/9.jpg)

9. Собрал докер 
> Блять, наконец-то

![image](images/10.jpg)

10. Ещё добавил скрипт на автовыполнение в 10:00 ~Спасибо Никите, этим поделился~

![image](images/12.jpg)

11. И docker + key(gey)cloak стартанулся

![image](images/11.jpg)

11. Роль + пользак

![image](images/14.jpg)

12. Затем созданной группе была создана роль.

![image](images/13.jpg)

12. Получение токена по паролю POST

![image](images/14.jpg)

13. Получение токена по refresh токену POST http://localhost:8080/realms/test/protocol/openid-connect/token 

![image](images/15.jpg)

14. Получение пользователей GET http://localhost:8080/realms/realm/protocol/openid-connect/userinfo

![image](images/16.jpg)

15. Получение информации про реалм GET http://localhost:8080/realms/test/.well-known/uma2-configuration

![image](images/17.jpg)

>P.S. На решение задачи было затрачено 2 дня, 5 банок энергетика, 10 часов музыки, 1 Никита и 1.5 миллиона нервных клеток