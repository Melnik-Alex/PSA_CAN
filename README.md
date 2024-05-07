# PSA_CAN
Decoding CAN-bus signals of Peugeot Citroen cars

# CAN 2010

### Impulse generator
I think, car takes that data from generator for understanding is engine started, or not.
This packet need for correct working CAN2010  and CAN2010EVO dashboards (it dimming STOP warning sign)
| Address        | Len           | Content  | Example  | 
| :-------------: |:-------------:| :-----| :-----:
| 0E6      | 8 | Voltage, timer | 00 00 00 00 00 81 80 84 |

### Base CAN packets

| Address        | Len           | Content  | Example  | 
| :-------------: |:-------------:| :-----| :-----:
| 036      | 8 | Eco, on/off, brightness | 0E 00 00 0F 31 07 05 AC |
| 0B6      | 8 | Speedometer, Tachometer | 4C F0 1E 00 FF FF FF FF |
| 0F6      | 8 | Engine temp, odometer   | 88 80 08 88 00 5B 78 20 |

| Address        | Len           | Content  | Example  | 
| :-------------: |:-------------:| :-----| :-----:
| 128     | 8 | Indicators - 1 | 20 30 04 00 08 00 04 00 |

| Byte | Bit        |  Content |
| :-------------: | :-------------: |:-------------:|
| 0 | 0 | Габариты |
| 0 | 1 | Ближний|
| 0 | 2 | Дальний|
| 0 | 3 | Передние ПТФ|
| 0 | 4 | Задние ПТФ |
| 0 | 5 | Правый поворотник |
| 0 | 6 | Левый поворотник |
| 0 | 7 | --- |
