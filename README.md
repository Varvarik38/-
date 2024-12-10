РЕПОЗИТОРИЙ КОМАНДНОГО ЗАДАНИЯ НТО КОМАНДЫ "ВАРВАРИКИ"

Шаг 1.
Клонирование репозитория из GitHub

Для клонирования репозитория из GitHub, следует изпользовать программу Git (GitBash)
Устанавливаем программу и видим терминал

![image](https://github.com/user-attachments/assets/5cb794e8-5bce-45d1-b3f6-35e872023185)

Создаём папку и копируем путь до неё. Затем изменяем все '\' на '/', т.к. Git поддерживает использование '/' символов

Далее следует открыть терминал и написать в нём:


cd (путь к папке)

Например:
cd C:/Users/varvariki

После ввода команды на терминале будет отображаться:

![image](https://github.com/user-attachments/assets/9f3eeb6a-6e6f-4d4b-83a5-20811e94806b)

Git перешёл в нужную директорию. Теперь можно клонировать репозиторий в папку.

git clone https://github.com/Varvarik38/-/new/main?readme=1




Шаг 1.
Настройка launch-ей в Виртуальной машине

После запуска Виртуальной машины заходим в папку Home. Последующий путь до нужных папок: 

"""
/home/catkin_ws/src/clover/clover/launch
"""

В папке launch открываем файл "clover.launch" через VS Code. В этом файле надо отредактировать параметр "aruco" и присвоить ему значение "true"

![image](https://github.com/user-attachments/assets/28229d73-9101-4be2-8169-1308d38c328d)

следующий нужный нам файл - aruco.launch . Путь до файла - /home/catkin_ws/src/clover/clover/launch/aruco.launch

параметры, которые надо поменять - "aruco_map" на "true"; "aruco_vpe" на "true"

![image](https://github.com/user-attachments/assets/43303d62-a769-4a13-b140-04f61c33e71e)



