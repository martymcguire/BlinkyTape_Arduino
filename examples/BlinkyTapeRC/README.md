# Erweiterte BlinkyTape Firmware für RC Modelle

Firmwareversion: 1.0
Hardware: BlinkyTape Board


Die Firmware unterstütz ein normales PWM Servosignal, und sollte mit jedem RC-Hersteller kompatibel sein.


Anschluss Servo Signal:

	5V = Pluspol (rot) 5V 
	A9 = Servo Signal (weiss)
	GND = Minuspol (schwarz)


ACHTUNG!! nur stabilisiertes BEC mit 5V verwenden und auf den Stromverbrauch achten.
Bei voller Helligkeit werden pro LED ca. 60mA benötigt, bei 100 LEDs sind dies bereits 6A !!


BlinkyTape per Servokanal steuern:

```
       RC-Position          Funktion
          
 +100%     +---+            -+
           |   |             |
           |   |             |-- BlinkyTape ON,
           |   |             |   Helligkeitseinstellung
           |   |             |
           |   |             |
           |   |  -- +5%    -+
    0%     +---+             |-- BlinkyTape OFF
           |   |             |
           |   |  -- -40%   -+      
           |   |             |
           |   |             |-- BlinkyTape ON,
           |   |             |   Farbmuster wechseln
           |   |             |
 -100%     +---+            -+ 
```



Releasnotes:

V1.0     15.01.17
- PWM Servosignal wird unterstütz
- Framedelay optimiert
