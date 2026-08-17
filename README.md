# Experiencia Guiada Sistemas de Información 2026-2

Todo el código de esta experiencia debe ser subido a un *fork* de este repositorio. Organice su trabajo en *branches* y haga un *merge* final una vez completados todos los puntos.

Realice las siguientes actividades.

- Publique una página web que indique su número de grupo y fecha. En este punto se recomienda fuertemente el uso de la plataforma [GitHub Pages](https://docs.github.com/en/pages) para su implementación, aunque puede realizarse de la manera que se desee.
- Lea una onda de voltaje sinusoidal, haciendo uso del generador de funciones del laboratorio, en su ESP32. ¿Cuál es la frecuencia de muestreo? Investigue posibles desafíos a la hora de adquirir el nivel de carga de un sistema de baterías.
- Busque información de la librería `SPIFFS` o similar para el almacenamiento de archivos en la ESP32. Guarde los datos de adquisición de 1 ciclo de la onda sinusoidal. ¿Al desconectar y volver a conectar su ESP32 sigue guardado el archivo? ¿Y al presionar `reset`, y `boot`?
- Busque métodos posibles para implementar filtros digitales a la señal adquirida. Entregue su señal filtrada a través de uno de los pines analógicos de la ESP32 usando el DAC, para observar su salida con un osciloscopio.
- Realice los siguientes 4 procesos en un solo flujo de código: Muestreo de la señal; Obtención de su FFT; Filtrado digital; Guardado en la memoria flash. Utilice la función `micros` para medir el tiempo de ejecución de cada proceso y grafique sus resultados. ¿Cuál es su 'cuello de botella'? Pruebe a variar algunos parámetros de sus funciones para entender qué procesos deben mantenerse simples, y cuáles tienen mayor flexibilidad (por ejemplo orden de los filtros, frecuencia de muestreo, etc.).
- ¿Qué precauciones debe tomar al cargar código al ESP-32 mientras está alimentada por baterías externas? ¿Qué consecuencias pueden haber si no se toman estas precauciones?
