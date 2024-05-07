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
| 036      | 8 | Eco, on/off, brightness | |
| 0B6 | 8      | Speedometer, Tachometer | |
| 0F6      | 8 | Engine temp, odometer | |

