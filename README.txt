# VkMusicDownloader
Получение юзер-агента
1.Сначала на устройстве проверяем, есть ли официальное установленное приложения вк.
2.Компилим и запускаем программу(app) 
3.В логах ищем: "USER_AGENT" и начиная от "VKAndroid..." до конца строки - ето и есть ваш юзерагент
Получение токена
1.Ставим MODE на 0.
2.Из примерно вот такого вывода:
{"access_token":"1234567"}
Ваш токен = 1234567
Потдверждения токена для аудио 
Более детально можна ознакомиться на https://habrahabr.ru
Как пользоваться:
1.Java
1.1 Подготовить данные
В файле Net.java меняем константы на свои
USERNAME - логин или номер телефона пользователя
PASSWORD - пароль пользователя
ACCESS_TOKEN - ваш токен.
USER_AGENT - ваш юзер агент
Поменять MODE на 1
1.2 
В командной строке перейти в папку: "ПутьКРепозиторию\ANDROID\"
ввести команду "gradlew fatJar"
Если все прошло ок, в папке "ПутьКРепозиторию\ANDROID\net\build\libs\" должен появиться jar-ник.
Осталось только запустить на Ubuntu-подобном команду
java -jar "ИМЯ ДЖАРНИКА"
2.На Python 
Там где пишет ТУТ_ЮЗЕР_АГЕНТ вставтье свой юзер-агент
Там где пишет ТУТ_ВАШ_ТОКЕН вставтье свой токен
