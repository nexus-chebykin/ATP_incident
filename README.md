# ATP_incident
**Battleship game** (_work in progress_) \
Классический морской бой. \
Предполагаются игра друг против друга (на одном компьютере), игра против бота. \
Интерфейсы: консольный и графический \
Сделано:
1) UML-диаграмма классов
2) Реализована эта структура классов
3) Реализованы методы внутренней логики
4) Реализован сценарий игры и консольный интерфейс
5) Реализована возможность игры с несколькими(>2) игроками
6) Реализованы боты различной сложности
7) Планы на будущее: 
- Реализовать более красивый консольный или графический интерфейс
- Улучшить алгоритм действия ботов
- Фичи, по типу торпед \ мин
___
Борис: 
- Диаграмма классов
- Player, Board, Ship, Cell

Семён: 
- Console GUI
- GameMaster, MenuDisplayer
- Settings

Обычный build через CMake (результат - игра в консоли): 
1) mkdir build && cd build
2) cmake ..
3) cmake --build .

Чтобы добавить GUI на SFML нужно 
1) На linux - установить SFML. Обычно для этого хватает установить libsfml-dev с помощью пакетного менеджера,
но если что-то не работает, обратитесь на официальный сайт: https://www.sfml-dev.org/tutorials/2.5/start-linux.php
2) На Windows и macOS библиотека установится за вас.
3) В шаге 2 обычного билда добавить -DUSE_GUI=ON.
___
Подсказки:
1) Чтобы повернуть корабль, покрутите колесиком мышки
2) Чтобы ввести настройку, нажмите enter