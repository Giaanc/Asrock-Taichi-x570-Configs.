# Asrock-Taichi-x570-Configs.

CSM Support -     Disable

BAR Resize -      Enable

4G Encode -       Enable

C-States Global - Disable

XMP -             Enable ( tRC 45* en Timings ) *Depende de la RAM*

AMD fTPM -        Disable (si es que estas en windows 10) (en windows 11, dependiendo de si parcheaste la instalacion se Activa, en el caso que no Desactivar)

Secure Boot-      Disable (si es que estas en windows 10) (en windows 11, si, activalo en conjunto con fTPM)

SVT AKA CPU Virtualizacion : Disable (aumenta el rendimiento L3 entre otros), la ultima version de windows 11 a la fecha (31/07 tiene reparado el error del L3, y contiene mejoras respecto al benchmark de AIDA64 

Ejemplo:

con cpu virtualización: https://gyazo.com/bc4ff93979c88d837c772fa51bd721a7

sin cpu virtualizacion: https://gyazo.com/0f7cfe932fdb37460fde1af20be078b0


Fan Settings:

CPU -             Full Speed (si es que el cabezal de la bomba del AIO esta en el cabezal CPU_FAN)

FAN4 -            Custom %45 (En las dos temperaturas (60 y 70))

# Opcional

PBO - Enable si tienes buen enfriamiento / Disable si es que no.

# OS 

Particion en GPT & Instalacion de windows en UEFI MODE

# Core Parking

ir a Regedit a la carpeta

HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\Power\PowerSettings\54533251-82be-4824-96c1-47b60b740d00\0cc5b647-c1df-4637-891a-dec35c318583

en el DWORD 'Attributes' y lo setean en 0, posterior en el plan de energia van a editarlo y podran ver el estacionado de cores (o core parking) sin programas externos.
no se recomienda bajarlo a menos del 25%, para CCD0 de amd es 50%
