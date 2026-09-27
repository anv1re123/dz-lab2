# Домашнее задание к работе 2

## Условие задачи

Определить путь, который проедут санки с горки высотой h метров, углом наклона `А` радиан и коэффициентом трения `k`.

## 1. Алгоритм и блок-схема

### Алгоритм

1. Начало.
2. Задать исходные данные:
   - `h` — высота горки, м;
   - `A` — угол наклона, рад;
   - `k` — коэффициент трения.
3. Вычислить `sin_A = sin(A)`.
4. Вычислить `cos_A = cos(A)`.
5. Вычислить условие движения санок:
   - `edut_vniz = sin_A - k * cos_A`.
6. Проверить условие `edut_vniz > 0`.
7. Если условие выполняется, вычислить путь санок:
   - `s = h / sin_A`.
8. Если условие не выполняется, вывести сообщение о том, что санки не будут скользить вниз.
9. Вывести результат.
10. Конец.

### Блок-схема

[Ссылка на блок-схему](https://viewer.diagrams.net/?tags=%7B%7D&lightbox=1&highlight=0000ff&edit=_blank&layers=1&nav=1&dark=auto#R%3Cmxfile%3E%3Cdiagram%20name%3D%22%D0%A1%D1%82%D1%80%D0%B0%D0%BD%D0%B8%D1%86%D0%B0-1%22%20id%3D%224AQj30h1wYhru1YKYX7c%22%3E3Vndb5swEP9rkLZJrfgOfWyabnvYpEl92PZUOXABrw5GxmmS%2FvUzxnwYSEtY2kbLQ%2BI739nmfr%2B7A2I4N%2BvdF4ay5DuNgBi2Ge0MZ2HYtuXYpvgpNPtS419ZpSJmOFJGjeIOP4FSKr94gyPINUNOKeE405UhTVMIuaZDjNGtbraiRN81QzH0FHchIn3tTxzxpNQG9qzRfwUcJ9XOln9VzqxRZayuJE9QRLctlXNrODeMUl6O1rsbIEXwqriUfp8PzNYHY5DyMQ45R4z3ndQ6Od9XlyzcRHSFMN8mmMNdhsJiZisAFrqEr4mQLDFc0ZTfKb9CzjmjD3WYnFpzQwllcm3HlJ%2FCFxPS0q%2FkR%2BjL0zwislGnMRamMV%2FIb9MQ2wSzaiy%2B5%2FL7VjkB47BrXZWKwxega%2BBsL0ySFlS%2BwmXbwGpVOrVKzV5FXleJSJEqrldu4i4GKvTDMOA024yCQfAlK4bCChEChMYMrUWEMmBY7AqsO%2FejmXgRObyDKtmsPhpgmaZEQ8cvpSko2Icg7UGXGLYIh3ld%2Fjy8FUrWKWCCKAaFSTE8mHMVbnTDwgq4JtHaWSVWqZKFMp7QmKaI3DbaOaObNIJi%2FyKajc03SjOF0x%2FgfK9wQxtOdVQPZ5sqnIjFwHs0bCfbIB4MCOL4UQ%2FCvwRXlNfwmVg2QdND8iKp9ZIShBCGx5IYERynQkdgxQtfsRtO429SWliDNM9xei84bkrJFNKH64%2BG7YtVpX1I89a0kPRpiDb8%2FjHFT%2B0VpMNFmTTmp9Kt0E1IoFk%2FgeqWpFaxr%2FQEOkmdK%2FhuT0ugFjfPN4FaHH6HBKJpNCp%2FErpebvKjcwf8ZYD6DUDMLAPP9cxjuoBGcNuPuTQyzUlsDgbaQdBpB5bOZsc7EZudaWxuEeWM2VwT6n26wX3%2B2u3AWiJLFKRx7eDw7Whel%2BlE8vlzU7BPdHfj6nS2OsXZnZ2Izvd7yCcyuibLuRCaoCWQOQofYrnJYSS7FbziXfeBw1UPGeMzQMF1YV66Gl7WM3CppX9QLKLdmNDVKgfew7M%2BwSiIqai6NcL%2F%2B5NGheKrZ593quxzpzeTirPnknz9zNK49%2FYNRVa3lB4R4TOJ5IgyJo7O9r%2BKzS9nllspfqvTSGGx06R9W2pl7mIYOxi6EWjewXjyHcwxSDaFMfCvfC2bLk5SHK8ZQ%2FuWRVZ45ANLqJN4Tqejep0XZy%2FY%2By%2FYu8%2Fbi0F54gPe5vDp6ssry4HymnCMeqES9d5CE3oNjHsaGf9iUW8SkQdB5A5lTmAvHd8%2FplNIEl%2Br14ZdWvuv1UacLhbBidqIN62NaAX6XKrfyFr0Kj1EiM2b%2BDIDmv8znNu%2F%3C%2Fdiagram%3E%3C%2Fmxfile%3E)
## 2. Реализация программы
Программа написана на языке **C++**.

```cpp
#include <stdio.h>
#include <locale.h>
#include <math.h>

int main()
{
    setlocale(LC_CTYPE, "RUS");
    // Задание исходных данных
    float h, A, k, sin_A, cos_A, edut_vniz, s;
    printf("Ввелите высоту горки:");
    scanf("%f", &h); // Высота горки, м 
    printf("Введите угол наклона:");
    scanf("%f", &A); // Угол наклона, рад
    printf("Ввелите коэффицент трения:");
    scanf("%f", &k); // Коэффициент трения 
    sin_A = sin(A); //Синус угла наклона
    cos_A = cos(A); // Косинус угла наклона
    edut_vniz = sin_A - k * cos_A;// Условие движения санок(сани поедут вниз если будет выполняться строгое неравенство)



    // Вывод данных
    printf("РАСЧЕТ ПУТИ САНОК С ГОРКИ\n");
    printf("================================\n\n");
    printf("ИСХОДНЫЕ ДАННЫЕ:\n");
    printf("- Высота горки h = %.2f м\n", h);
    printf("- Угол наклона A = %.2f рад\n", A);
    printf("- Коэффициент трения k = %.2f\n", k);
    printf("РАСЧЕТ:\n");


    // Условие движения санок
    if (edut_vniz > 0) // Санки едут вниз, т.к. сила трения позволяет им начать движение 
    {
        s = h / sin_A; // // Формула определения пути 
        printf("- sin(A) = %.4f\n", sin_A);
        printf("- cos(A) = %.4f\n", cos_A);
        printf("- Условие движения: sin(A) - k*cos(A) = %.4f\n", edut_vniz);
        printf("================================\n");
        printf("ДЛИНА ГОРКИ:\n");
        printf("s = h / sin(A) = %.2f / %.5f = %.2f м\n\n", h, sin_A, s);
        printf("ОТВЕТ: Санки проедут %.2f м.", s);

    }
    else // Санки не поедут вниз, т.к. сила трения не позволяет им начать движение 
    {
        printf("Строгое неравенство не выполняется: %.4f<0\n", edut_vniz);
        printf("================================\n");
        printf("ОТВЕТ: Cанки не будут скользить вниз,т.к. сила трения не позволяет им начать движение.");
    }

    return 0;
}
```
## 3. Результаты работы программы
```text
Ввелите высоту горки:10
Введите угол наклона:1
Ввелите коэффицент трения:2
РАСЧЕТ ПУТИ САНОК С ГОРКИ
================================

ИСХОДНЫЕ ДАННЫЕ:
- Высота горки h = 10.00 м
- Угол наклона A = 1.00 рад
- Коэффициент трения k = 2.00
РАСЧЕТ:
Строгое неравенство не выполняется: -0.2391<0
================================
ОТВЕТ: Cанки не будут скользить вниз,т.к. сила трения не позволяет им начать движение.
```
## 4. Информация о разработчике
```text
Имя: Коноавленко Ярослав
Вариант: 13
Группа: бИЦТ-261
Подгруппа: 1
