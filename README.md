## Описание шагов pipeline

Начинаем со сборки проекта, устанавливаем необходимые пакеты и зависимости.
Затем тестируем код по PSR и покрываем юниттестами (плюс собираем артефакты). При этом ошибки по PSR не являются критическими по политике отдела, поэтому этот шаг не является критичным.
Затем билдим докер для запуска либы и проверяем его на работоспособность.
Далее выгружаем образ в хаб (этот этап упадет в ошибку, т.к. указаны фейковые данные).
