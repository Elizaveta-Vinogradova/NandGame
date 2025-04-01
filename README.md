# Smile Race

## Краткое описание игры

**Smile Race** - это платформер, в котором персонаж-шарик должен перепрыгивать через стены. В каждом забеге у игрока есть возможность использовать 2 способности: F2 - включает неуязвимость на 3 столкновения, поэтому шарик не разобьется, F3 - сбрасывает скорость до дефолтной. Кстати, о скорости: с каждой сотней набранных очков она увеличивается.

## Запуск игры

1. Загрузи все файлы из каталога **src** себе на компьютер.
2. Открой **VMEmulator.bat(.sh)** и загрузи папку с файлами игры.
3. Отключи анимацию (Animate -> **No Animation**) и выбери режим **Fast**
4. Запусти игру, нажав двойную стрелочку в левом верхнем углу экрана.
5. Наслаждайся процессом!

## Технические особенности игры

В ходе реализации мы столкнулись с проблемой переполнения стека в ходе игры. Причиной этой ошибки оказалось создание строки "Current score: " сразу в методе Output.printString. Дело в том что этот метод содержался в цикле while, и мы каждую итерацию пересоздавали эту строку. Решение, конечно, самое простое: вынести "Current score: " в переменную перед циклом.

## Авторы

Игра создана в рамках курса **NandToTertis** студентами ФТ-104:
- Гусаров Иван
- Курзаев Данила
- Веселков Дмитрий
