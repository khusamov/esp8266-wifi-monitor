# Wi-Fi монитор на ESP8266

Группа для сбора информации по проекту:
https://vk.com/club204372209

![image](https://user-images.githubusercontent.com/4146998/196043494-1aaf2ac6-11bc-4f88-ac91-01ca3d7538b2.png)

Состав проекта:
---------------
- Монитор от домофона с интерфейсом AV (TV).
- Arduino Nano в качестве видео-адаптера для этого монитора.
- ESP-01 в качестве основного контроллера.
- Level converter для согласования уровней между ESP и Nano.
- Понижающий адаптер DC-DC с 12В до 3.3В для ESP.
- Разъем для 12В адаптера питания.
- Спец-кабель для соединения монитора и Nano.

Питание Ардуино Нано: нерегулируемое напряжение 6-20V (вывод 30, Vin).
Питание ESP-01: через Mini360 DC-DC понижающий до стабильных 5V.
Соединение ESP-01 с шиной GyverBus через согласователь уровней 3V3/5V.

Внутрисхемная связь
-------------------

Arduino Nano и ESP-01 предполагается связать при помощи GYVERBUS
https://alexgyver.ru/gyverbus/
Если это не получится, то есть еще несколько вариантов как связать.

Данная связь нужна для передачи кадра на монитор.

Программирование ESP-01
----------------

https://portal-pk.ru/news/241-obzor-usb-adaptera-programmatora-dlya-esp-01-na-ch340g.html

Ссылки
------

Схема проекта:
https://easyeda.com/editor#id=31b8b3f701ac42ca969ea86ee8b71cc9

Библиотека TV-out:
https://github.com/Avamander/arduino-tvout
