# simple_person_detector
This simple app is based on MobileNet network and gives opportunity to detect some people on the frame

Данный код позволяет находить людей в кадре, используя обученную нейронную сеть(MobileNet network)

Всего представлено два варианта:
    1)Однопоточное приложение, исползующее один видедевайс
    2)Многопрцессорное приложение(удалось обрабатывать одновременно 4-5 потоков)

Эксперименты с многопроцессроным вариантом проводились на следующем оборудовании:  
    1) i5-5300U (2 ядра - 4 потока)
    2) Intel Corporation HD Graphics 5500
    3) 8 гигабайт озу
Основной упор был именно в ЦПУ.

Примерный результат работы приложения:

<p align="center">    
<img src="https://github.com/birallex/simple_person_detector/blob/main/example.png" width="720" height="480"/>
</p>