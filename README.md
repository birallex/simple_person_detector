# simple_person_detector
This simple app is based on MobileNet network and gives opportunity to detect some people on the frame

## Микрообзор:

Данный код позволяет находить людей в кадре, используя обученную нейронную сеть(MobileNet network)

Всего представлено два варианта:
1. Однопоточное приложение, исползующее один видедевайс
2. Многопрцессорное приложение(удалось обрабатывать одновременно 4-5 потоков)

Эксперименты с многопроцессроным вариантом проводились на следующем оборудовании:  
1. i5-5300U (2 ядра - 4 потока)
    - Основной упор был именно в ЦПУ
    - Существует вероятность высого нагрева цп
2. Intel Corporation HD Graphics 5500
3. 8 гигабайт озу
    - Разницы с 4 гигабайтами озу замечено не было

## Работа скрипта:

Примерный результат работы приложения:

<p align="center">    
<img src="https://github.com/birallex/simple_person_detector/blob/main/example.png" width="720" height="480"/>
</p>

## Запуск

Запуск может быть произведён с помощью следующих команд:
- `python3 detect_person.py`
- `python3 multiprocessing_person_detector.py`