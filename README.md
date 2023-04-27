# YoptaC
Инновационный язык программирования для четких пацанов на основе C++

YoptaC - это первый в мире статически типизированный язык программирования для гопников и четких пацанов, основанный на макросах C++.
Синтаксис языка прост и использует понятные для гопоты слова, позволяя им быстро начать разработку.
Свои предложения по синтаксису можете писать в issue. Язык находится в начальном этапе разработки и конечный стандарт ещё не определён.
Однако уже сейчас его можно использовать для написания консольных приложений.

## Создание проекта на YoptaC
1. Создать консольное приложение c++ в Visual Studio
2. Добавить в проект файл заголовков YoptaC.h
3. Подключить заголовки командой ```#include "YoptaC.h"```
4. Готово! Теперь вы можете создавать свои программы на YoptaC.

## Пример
Программа для вычисления корней квадратного уровнения.

```c++
#include "YoptaC.h"

куку main() жЫ
    русский нах
    крымнаш нах
    сказать("Работает на YoptaC++\n") нах
    букавы имя нах
    сказать("Куку ёпта! Как тебя звать, бедолага?\n") нах
    говори чё имя нах
    базарить бля имя бля ", тебе решить квадратное уравнение? Введи параметры a, b, c" бля конец нах
    чёткий a, b, c нах
    говори чё a чё b чё c нах
    хули(a неровно 1) базарить бля a нах
    базарить бля "x^2" нах
    хули(b нехуёвей 0) базарить бля "+" нах
    хули(b неровно 1) базарить бля b нах
    базарить бля "x" нах
    хули(c нехуёвей 0) базарить бля "+" нах
    базарить бля c бля " = 0" бля конец нах
    чёткий D = b*b - 4*a*c нах
    базарить бля "D = " бля D бля конец нах
    хули(D нехуёвей 0) жЫ
        число x1 = (-b + корень(D)) / 2*a нах
        число x2 = (-b - корень(D)) / 2*a нах
        базарить бля "x1 = " бля x1 бля конец нах
        базарить бля "x2 = " бля x2 бля конец нах
    всё
    огребаешь
        сказать("соси, дискриминант меньше 0") нах
всё
```

Оригинальный код на C++
```c++
#include <iostream>
#include <string>
#include <Windows.h>

void main() {
    SetConsoleCP(1251);
    SetConsoleOutputCP(1251);
    printf("Работает на YoptaC++\n");
    std::string имя;
    printf("Куку ёпта! Как тебя звать, бедолага?\n");
    std::cin >> имя;
    std::cout << имя << ", тебе решить квадратное уравнение? Введи параметры a, b, c" << std::endl;
    int a, b, c;
    std::cin >> a >> b >> c;
    if (a != 1) std::cout << a;
    std::cout << "x^2";
    if (b >= 0) std::cout << "+";
    if (b != 1) std::cout << b;
    std::cout << "x";
    if (c >= 0) std::cout << "+";
    std::cout << c << " = 0" << std::endl;
    int D = b*b - 4*a*c;
    std::cout << "D = " << D << std::endl;
    if (D >= 0) {
        float x1 = (-b + sqrt(D)) / 2 * a;
        float x2 = (-b - sqrt(D)) / 2 * a;
        std::cout << "x1 = " << x1 << std::endl;
        std::cout << "x2 = " << x2 << std::endl;
    }
    else
        printf("соси, дискриминант меньше 0");
}
```