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

git clone https://github.com/Varvarik38/NTO_Varvariki.git


Шаг 2.
Установка Виртуальной машины и симулятора Gazebo

Чтобы установить Виртуальную машину настроить её, предлагаем видео-инструкцию с оффициального ютуб-канала Coex:

https://youtu.be/-4TUYInDg5w?si=oF7AFUv50E1ugFKg

а так же инструкцией:

https://clover.coex.tech/ru/simulation_vm.html

Шаг 2.1.
Установка объектов на виртуальную машину

Перед созданием мира Gazebo надо установить объекты из репозитория Бартова Артёма.

https://githud/com/bart02/dronepoint

После скачивания открываем Виртуальную машину и переходим в нужную папку по пути:

catkin_ws/src/clover/clover_simulation/models/

и переносим в эту папку следущие объекты (из репозитория Артёма Бартова):


dronepoint_blue
dronepoint_green
dronepoint_red
dronepoint_yellow


![image](https://github.com/user-attachments/assets/3ab49e41-2a1c-4ad4-bb5c-4deba4ed88fe)

Шаг 2.2
Настройка симулятора

При желании можно самостоятельно настроить launch-и (см. 2.2.1)
Для автоматической настройки симулятора создаём файл, содержащий код, который проводит автонастройку симулятора и рандомно генерирует карту.

!!!Код содержится в файле Varvariki.txt в репозитории по ссылке:

https://github.com/Varvarik38/generation_code_Varvariki.git



Шаг 2.2.1. (необязательно)
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



