# ROBO Pro Coding Python Dokumentation

## Controller

### Initialisierung und Erzeugen eines Controllers

```python
import fischertechnik.factories as txt_factory

txt_factory.init()

txt = txt_factory.controller_factory.create_graphical_controller()

txt_factory.initialized()

```
### Input

**Initialisierung Input Factory**
```python
txt_factory.init_input_factory()
```

**Erzeugen eines Mini-Tasters an I1**
```python
mini_switch = txt_factory.input_factory.create_mini_switch(txt, 1)
```
**Erzeugen eines NTC-Widerstands an I1**
```python
ntc_resistor = txt_factory.input_factory.create_ntc_resistor(txt, 1)
```
**Erzeugen eines Fotowiderstands an I1**
```python
photo_resistor = txt_factory.input_factory.create_photo_resistor(txt, 1)
```
**Erzeugen eines Fototransistors an I1**
```python
photo_transistor = txt_factory.input_factory.create_photo_transistor(txt, 1)
```
**Erzeugen eines Ultraschall-Abstandssensors an I1**
```python
ultrasonic_distance_meter = txt_factory.input_factory.create_ultrasonic_distance_meter(txt, 1)
```
**Erzeugen eines optischen Farbsensors an I1**
```python
color_sensor = txt_factory.input_factory.create_color_sensor(txt, 1)
```
**Erzeugen eines IR-Spursensors an I1**
```python
trail_follower = txt_factory.input_factory.create_trail_follower(txt, 1)
```
### Motor

**Initialisierung Motor Factory**
```python
txt_factory.init_motor_factory()
```

**Erzeugen eines Motors an M1**

```python
motor = txt_factory.motor_factory.create_motor(txt, 1)
```

**Erzeugen eines EncoderMotors an M1**

```python
encoder_motor = txt_factory.motor_factory.create_encodermotor(txt, 1)
```

### Output

**Initialisierung Output Factory**
```python
txt_factory.init_ouput_factory()
```

**Erzeugen einer LED an O1**

```python
led = txt_factory.output_factory.create_led(txt, 1)
```

**Erzeugen eines Magnetventils an O1**

```python
magnetic_valve = txt_factory.output_factory.create_magnetic_valve(txt, 1)
```

**Erzeugen eines Kompressors an O1**

```python
compressor = txt_factory.output_factory.create_compressor(txt, 1)
```

**Erzeugen eines unidirektionalen Motors an O1**

```python
unidirectional_motor = txt_factory.output_factory.create_unidirectional_motor(txt, 1)
```
### Servomotor

**Initialisierung Servomotor Factory**
```python
txt_factory.init_servomotor_factory()
```

**Erzeugen eines Servomotors an S1**
```python
servomotor = txt_factory.servomotor_factory.create_servomotor(txt, 1)
```

## Counter / Digital Input

**Initialisierung Counter Factory**
```python
txt_factory.init_counter_factory()
```

**Erzeugen eines Encodermotor Zähler an C1**
```python
motor_step_counter = txt_factory.counter_factory.create_encodermotor_counter(txt, 1)
```
**Erzeugen eines Mini-Tasters an C1**
```python
mini_switch = txt_factory.counter_factory.create_mini_switch_counter(txt, 1)
```

## I2C

**Initialisierung I2C Factory**
```python
txt_factory.init_i2c_factory()
```
**Erzeugen eines Gestensensors**
```python
gesture_sensor = txt_factory.i2c_factory.create_gesture_sensor(txt, 1)
```
**Erzeugen eines Umweltsensors**
```python
environment_sensor = txt_factory.i2c_factory.create_environment_sensor(txt, 1)
```
**Erzeugen eines Kombisensors**
```python
combined_sensor = txt_factory.i2c_factory.create_combined_sensor(txt, 1)
```
