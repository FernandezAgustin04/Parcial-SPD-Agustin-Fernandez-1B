# Parcial-SPD-Agustin-Fernandez-1B 

-Agustín Fernández

# MONTACARGAS
Este proyecto consiste en un código para controlar un elevador de pisos utilizando Arduino. El sistema cuenta con botones para subir, bajar y detenerse, así como LEDs indicadores y un display de 7 segmentos para mostrar el piso actual.
![Tinkercad](./img/ArduinoTinkercad.jpg)


## Pines utilizados
- `ledVerdePin`: Pin utilizado para el LED verde.
- `ledRojoPin`: Pin utilizado para el LED rojo.
- `displayAPin` a `displayGPin`: Pines utilizados para controlar los segmentos del display de 7 segmentos.
- `botonSubirPin`: Pin utilizado para el botón de subir.
- `botonBajarPin`: Pin utilizado para el botón de bajar.
- `botonDetenerPin`: Pin utilizado para el botón de detener.

## Variables
- `contador`: Variable utilizada para almacenar el número de piso actual.
- `pisoAnterior`: Variable utilizada para almacenar el piso anterior.
- `ultimoEstadoSubir`, `ultimoEstadoDetener`, `ultimoEstadoBajar`: Variables utilizadas para el debouncing de los botones.
- `ultimoTiempoDebounce`: Variable utilizada para almacenar el último tiempo de debounce.
- `debounceDelay`: Valor utilizado para determinar el tiempo de debounce.

## Funciones
- `setup()`: Función de configuración que se ejecuta una vez al inicio del programa. Configura los pines de los LEDs, el display y los botones.
- `loop()`: Función principal que se ejecuta en un ciclo continuo. Lee el estado de los botones, realiza el debouncing y controla el funcionamiento del elevador.
- `mostrarMensajePiso()`: Función que muestra en el Monitor Serial el número de piso actual.
- `displayNumero()`: Función que controla el display de 7 segmentos para mostrar el número de piso actual.
- `apagarDisplay()`: Función que apaga todos los segmentos del display.

