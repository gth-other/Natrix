# Natrix
**Natrix** - шахматный движок с графическим интерфейсом.<br><br>
Уровень игры движка оценивается приблизительно в **2000** Эло.<br><br>
Если у Вас **deb** дистрибутив **Linux**, то Вы можете установить программу из готового **deb** пакета.
![logotype](data/UI/images/logotype.png)
## Зависимости
* **SDL2**
* **SDL2_Image**
* **SDL2_Mixer**
* **SDL2_TTF**
## База дебютов
Этот движок использует базу дебютов.<br><br>
Используемая база дебютов является файлом на несколько тысяч строк, каждая из которых содержит по **12** ходов в длинной нотации (например - **e2e4**).<br><br>
В коде не зашито количество строк в базе или количество ходов в одной строке, так что Вы можете расширять (уменьшать) базу дебютов без повторной сборки проекта и каких-либо изменений в коде. <br><br>
Учтите, что база целиком загружается в память, так что очень большие базы не рекомендуются.<br><br>
При загрузке базы в память проверяется легальность ходов из базы. При найденных ошибках в базе запуск прерывается.