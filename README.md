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

### What is what

| Address        | Len           | Content  | Description  | 
| :-------------: |:-------------:| :-----| :-----:
| 169      | 8 | Navigation info | Non-graphical navigation data like compass etc. |
| 2E9      | 4 | Additional functions | Dashboard theme, personalisation |
| 328      | 2 | 01 30  | Radio OFF  |
|       | 6 | 05 00 01 04 52 00 | Radio ON - just radio |
|       | 8 |  | Radio with RDS |
|       |  |  |  |
|       |  |  |  |
