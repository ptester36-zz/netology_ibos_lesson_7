# 1. Какое предупреждение (Warning) было выведено при компиляции? По желанию: проведите доп.исследование на предмет сути предупреждения (с чем оно связано, какие риски от использования одной из функций в программе и что это за функция).

Суть предупреждения:

Программист должен знать максимум числа символов, которые должны быть считаны gets, чтобы удостовериться, что выделяется буфер достаточного размера. Подобное невозможно без информации о данных. Эта проблема может приводить к созданию ошибок и открывает простор для нарушений компьютерной безопасности при помощи переполнения буфера.

Вместо gets могут быть использованы другие функции строкового ввода, что позволит избежать ошибок, связанных с переполнением буфера. Простейшим вариантом будет fgets.

![](/pic/um.png)

# 2. Ввод, приводящий к падению приложения

Переполнение переменной "Command" через переполнение gets

![](/pic/dois.png)

# 3. Ввод, приводящий к выполнению другой команды (не ping)

Перезапись переменной "Command" через переполнение gets (14 пробелов + ls)

![](/pic/tres.png)