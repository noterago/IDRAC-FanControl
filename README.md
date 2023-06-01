# IDRAC-FanControl
Ręczne sterowanie obrotami wentylatorów serwera

Zainstaluj: apt install ipmitool !!


Zaloguj się do Idraca

![image](https://github.com/noterago/IDRAC-FanControl/assets/120764107/fcce2729-35d1-4be3-9c68-91a53ee0357e)

Przechodzimy do zakładki Idrac Settings / Network i wybieramy u góry IPMI Settings

![image](https://github.com/noterago/IDRAC-FanControl/assets/120764107/c6866f3d-e3f4-4cdc-b1ee-0ca94c0598f3)

I uruchamiamy IPMI Over LAN

![image](https://github.com/noterago/IDRAC-FanControl/assets/120764107/e1fde2f7-19d8-4244-8512-cee112081973)

Teraz wystarczy zalogować się do konolki i wywołac komende by uruchomić ręczne sterowanie: ipmitool -I lanplus -H Idrac-IP -U twoje-hasło -P slaw raw 0x30 0x30 0x01 0x00
