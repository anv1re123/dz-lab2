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

[Ссылка на блок-схему](https://viewer.diagrams.net/?tags=%7B%7D&lightbox=1&target=blank&highlight=0000ff&edit=_blank&layers=1&nav=1&title=%D0%A1%D1%85%D0%B5%D0%BC%D0%B0.drawio&dark=auto#R%3Cmxfile%3E%3Cdiagram%20name%3D%22%D0%A1%D1%82%D1%80%D0%B0%D0%BD%D0%B8%D1%86%D0%B0-1%22%20id%3D%22GmaI5vad0gJjucbkHoGs%22%3E7Vzrb6M4EP9rIrUnFRnz%2FphHu3vS3e3qetJ9XNHETVAJ5ID0sX%2F9DdgmNpgEaEgfm2o3IePXeGbs39gzyciYrp%2B%2FJP5m9We8IOEIo8XzyJiNMNYNjOAtp7xQiu3plLBMggWrtCPcBj8JI7J2y22wIKlUMYvjMAs2MnEeRxGZZxLNT5L4Sa52H4fyqBt%2FSWqE27kf1qn%2FBotsRakudnb0ryRYrvjIuu3RkrXPK7OZpCt%2FET8JJON6ZEyTOM7o0%2Fp5SsJceFwutN1NQ2nJWEKirE0D%2FNeD%2Be3b37f%2FZD%2B%2Fzr5u11fO7PuV7ta7YT2n2QsXQhJvowXJ%2B0EjY%2FK0CjJyu%2FHneekTqB1oq2wdwicdHtMsiR%2FINA7jpGhtTMZTd2ZAyX0cZQL9uvjL6UEYCnTkWZY1ATrl49EPt4wPRiBJRp4FXtl8v5B4TbLkBaqsJJVYtN3TTn%2BGjjSXqZD1hG1Hc9nUma0apsEMiRnRshxhJ2d4YKLuIvY2Uod%2BwMpJC4mv%2FA35PUphpTBK6N%2BRcOLPH5aF6rhwozgie%2BTdXXM7w9CPpy%2BEavrSXVuzJHUZBpJ0xfeLo6sKt1EVzC%2BTdaJSmSxfhTIYyQ%2BDZQQf5zAiAfokl2AAe9KYFayDxSIfuiL%2FA1pv0KFCa3aYsQbSNO3%2FtjEvuEqLrXoMFbC1eS764eXwtGTvRUd3VUJQEmBD8Wb56wSNYA6wJtkzvBalk2veCLQXVDsCWq1zoFHOObmHDdoKE%2BRmyQ3QMTRsyfvFUDZotLHBYheAR6jlhyEJ42Xir0EAG5IEwEZuSHLZ911B9x3mPngmHK4%2F445TKpOrG7lVdevuUPo2ab9kUfNN9uJFtBjnHk%2B%2Bc4R%2BmgZzWYldNouaYtDEnNnjimIW5N7fhlmTIvZL3WLSS0joZ8GjPFNBE9YeKRcjwKT9F6HCJg6iLBUY%2BJ4Tdqo0MdaciiotVFEa7bR9B7jCZRpvkzlhDUWvrEVfTqWvzE%2BWJKv1VZhWKdz%2B1mZ1QLjjQ1gKm04QLf8g9%2FnY5o7yNzOVnBRD8%2FuwMO0VNCRRvq9RNQN3sJVYgBl4isBJsIDbKXzWd5%2FhX149AbuNYAJ%2BUEyT%2BGn2RNKsWBmZn%2Fl3xVxbeLj9cPbgztUNdfX2qJuDLC7AFDNIzV9hk0HsYYe5M%2F4KWDwpXq1iuA5wS8mL4LFKGmBmh3qu97ECs4BBpg%2FwPw2iH%2FnzPE6Ld7LYZj8eo%2BBnXnZgfndJL1%2BkUTgKknIIRb121COdnIBa7lccGnVbM70TQaN9hsbTQqOBXwmN2DseNBrmaaGRnyrP2PixsNHpio0l3NEDqFs868Ix1BLg0SW8H1BHpGTorpTA1ZzON%2BcL5Bul3JYmxa1lWRbmKr1a%2BMnDRbK8u8hVBlT%2Bdknf8xJsWfSD%2BHB5qZ6vhN2U22Oi1vEVQjHZmMH7xfiyB5dqNDwJ79SPgIUdpx%2BO953vU8g%2B94fQFfx%2F%2BI15R6%2BezJAHc1NGiX24%2BLp7W3x2P07rfpjeK90P0z6e%2B2FVb5mHdj9aXfwlq3h9t00PY%2FMnixMYiktaux4nsGtarN7VHG97MAd0F8PCCzw7i8d2FrHeP3zR%2Ff5BuGNoQk9%2FnYup%2BAQyvHmL%2BIelWFoWKi%2FA%2BdoyXXlhVbfa4y0s64y7A%2BKuwXGNK9K19kIjNvfWPwDSZU5IpXVnhK6yYeveaeHZOYFVzrfJY5l68euaqL3fRA%2BYnGUcyeSqbNhVX2Jok%2FNaeYSfLV8HV4Lvuok0JCfr2INF33GrS8APLXNVwkNV5haqJTwMKPNWO%2Bk55aH3IlMp3HSrHh6sRc2VnTx3sNMTn8rZyRsEQbHhaZa8Zzp2FxBVdWD2dd0UfXmVvgaGUtzqcuXtM%2FvQnq1BYX%2FlmVVxHD0YbpBCCruQg6q0IeCQx1N4QoHykNpjs1Jc9NgyNolbF3fxBrsExl1ueT6a4ShzHToak45wxWB0x%2BtvTjMegNNHLh765uOwrVnGKW2tS3LWR7O19nk81bCW3XRl1yucyygsHeqmqGwwc6MVMBJ6EDOlaCrVWI6zNkTDatNV5fwcXSTUItEqnwOYInRFo3uduR0qntfkdaLdX%2FWk52jWUOvNOa83hXE1hpGl9VYmGFp8tQhL6O1XSNMkruiikEP2fVfFifmupRp8EL5bhEHeK%2BtwxEIXgp87EUCEf5WlGUo%2BmK4E2LsWXunS9hqhtNdif8tp7igwgXEd58eCI1AqFgkSsXgqtaBwaitFwVSTBn0L7FWFyz2jhr31m1XXGAxtW3379JdDW%2FczoG3TJN472u7j%2Bz2j7T6%2B3znaNrE%2B%2FzS407iiS8r0EOTwWxD2UedIo0AdAbTHgvAomNOBxHMxZnTWM67J1aHXNLSyxuuNNXkoV%2FCGUFldAMqKwoB%2B0zC5G4Frp%2FbFpQlrK90KIYGHqdxt5ZvF9RmbwhC0B7v5kuBtUVx1P6VAcQs58pG5ek9%2FPAhnAelBgzbNYRkF%2Br7fAEwlXUVHcm5rPVEGdWxQXlU2NDgU4Kkw6PX95o7RxMepYjt8lZytskViTS2s77n7zUzRpKOlqQat5la3NTYLN3NzMnsb%2BgddDljeO0zZUeWL2qbGU9pLTQ33oxn4fLisu6J47%2BFSdBfFsJvdydvpYUGOwoAw0hxTNiDH1dzKN41Rj9gbfNz97hbdA3a%2FXmZc%2Fw8%3D%3C%2Fdiagram%3E%3C%2Fmxfile%3E)
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
