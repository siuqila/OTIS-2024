### Лабораторная работа №2
#### ПИД-регуляторы
####  Скачков Евгений Владимирович
#### Для чего нужен этот код 
Реализовывает программу, моделирующую рассмотренный выше ПИД-регулятор.
#### Функция данного кода
Функция определяет три переменные (q0, q1, q2), которые зависят от  параметров (K, TD, To, T)
```C++
void unlinear(double value) {

    int t = 100;

    double q0 = K * (1 + TD / To);

    double q1 = -K * (1 + 2 * TD / To - To / T);

    double q2 = K * TD / To;
```