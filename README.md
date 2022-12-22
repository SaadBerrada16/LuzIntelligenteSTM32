# Controlador de Luz Intelligente

El Controlador de Luz Intellige es un sistema de monitoreo y control de luz a través de sensores implementado en mBed OS utilizando como placa de desarrollo la placa STM32F401 conocida como la "blackpill". Este proyecto se compila y se executa con el IDE STM32CubeIDE

El proyecto se realiza en el marco del trabajo final de la materia Sistemas Embebidos de la Facultad de Ingeniería de la Universidad de Buenos Aires.

[Repositorio](https://github.com/SaadBerrada16/LuzIntelligenteSTM32)

[Definición de Requisitos y Casos de Uso del Trabajo Final](https://docs.google.com/document/d/1cPnTIswwUo-lCDzXssSQgjeIAEjO98fRAwfNpBX1VfY/edit?usp=sharing)

## Descripción y diagrama en bloques

En este trabajo se explica el diseño y armado de un controlador de luz inteligente. Este controlador debe permitir encender y apagar una luz de diferentes maneras usando sensores. Se puede manejarla con un sensor de presencia infrarrojo, un sensor de sonido, y un sensor de movimiento.

Por su comodidad, este de luz controlador podría tener una utilización personal futura a este proyecto. En efecto, podría ser conectado a una luz en su domicilio para controlarla a distancia o automáticamente.

<p align=center>
    <img src="docs/images/block_diagram.png" alt="Diagrama en bloques del proyecto" height="350"/>
</p>![Interfaz con el usario)](https://user-images.githubusercontent.com/116112545/209142978-88f9ee47-9688-4450-ac84-6dfb961be0bc.png)


## Organización del repositorio

El repositorio se organiza con la siguiente estructura

    .
    ├── Core
    │   ├── Inc
    │   |   ├── main.h
    │   |   └── ...
    │   ├── Src
    │   |   ├── main.c
    │   |   └── ...
    │   └── Startup
    ├── Debug
    │   └── ...
    ├── Drivers
    │   └── ...
    ├── LuzIntelligente.ioc
    ├── README.md
    └── ...


En donde se tienen las carpetas o archivos:
* `Core/`: carpeta que incluye las carpetas Inc, Src, y Startup. La carpeta Inc contiene los .h del proyecto y Src contiene los archivos principales del programa del sistema.
* `esp32_wifi/`: carpeta que contiene los archivos fuente utilizados para programar la placa ESP32 utilizada como módulo Wi-Fi y controlada a través de puerto serie.
* `modules/`: carpeta que contiene los archivos fuente de los distintos módulos que integran el programa del sistema.
* `main.c`: archivo principal del programa del sistema.
* `README.md`: este archivo *read me*.
* Otros archivos tales como licencia, archivos de configuración de mBed OS, etc.
