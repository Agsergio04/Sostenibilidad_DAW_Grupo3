## Cómo Convertir la Raspberry Pi en un NAS

### Materiales Necesarios

- **Raspberry Pi** (modelo 3 o superior recomendado).
- **Adaptador de corriente** (2.5 A para Raspberry Pi 3).
- **Tarjeta microSD** (mínimo 8 GB).
- **Unidad de almacenamiento externa** (pendrive o disco duro USB).
- **Software**: Raspberry Pi Imager.

### Instalación del Sistema Operativo

1. **Descarga e instala** Raspberry Pi Imager.
2. **Selecciona la versión** de Raspberry Pi OS y escribe en la tarjeta microSD.
3. **Inserta la microSD** en la Raspberry Pi y realiza la configuración inicial.

### Instalación de Open Media Vault

1. **Abre la terminal** y ejecuta el siguiente comando para instalar Open Media Vault:
   ```bash
   wget -O - https://github.com/OpenMediaVault-Plugin-Developers/installScript/raw/master/install | sudo bash


# Raspberri Pi:

Por lo general una Raspberri Pi4 consume en torno a 0.5 - 1 A/h 

Promedio de consumo 1.5 A/h

 ## Especificaciones : 
 ### Raspberry Pi 4

Procesador ARM Cortex-A72

Frecuencia de reloj 1,5 GHz

GPU VideoCore VI (con soporte para OpenGL ES 3.x)

Memoria 1 GB / 2 GB / 4 GB LPDDR4 SDRAM

Conectividad Bluetooth 5.0, Wi-Fi 802.11ac, Gigabit Ethernet

Puertos  GPIO 40 pines 2 x micro HDMI 2 x USB 2.0 2 x USB 3.0 CSI (cámara Raspberry Pi) DSI (pantalla tácil) Micro SD Conector de audio jack USB-C (alimentación)

### Raspberry pi zero w

dimensiones y peso 65 x 30 mm

16 gramos procesador

Broadcom BCM2710A1 Cuatro núcleos ARM Cortex-A53 a 1 GHz Memoria RAM 512 MB LPDDR2

conectividad Wi-fi 2,4 GHz 802.11b/g/n Bluetooth 4.2 (BLE) 1x Micro USB 2.0 (OTG) 1x Mini HDMI 1x Micro USB para la alimentación

Toma de E/S GPIO de 40 pines Ranura para tarjetas microSD Conector de cámara CSI-2

multimedia Descodificación H.264, MPEG-4 (1080p30)

Codificación H.264 (1080p30) Gráficos OpenGL ES 1.1, 2.0 otros Pines de vídeo compuesto y reset mediante puntos de soldadura de texto

## Placa Solar
Teniendo en cuenta que tenemos una raspberry que consume 1.5 A/h tenemos que en un dia a pleno funcionamiento (1.5 A/h * 24 h/dia = 36 A/dia ) nos daria un total de 36 A/dia siendo que necesitaremo para almacenar la energia minima de 1 mes seria de 1080 A/mes.

Por otro lado 
por lo que teniendo en cuenta una placa solar de 100 W 


# Raspberry Pi y Energía Solar

## Consumo de Energía de Raspberry Pi

Para una Raspberry Pi 4 que consume un promedio de 1.5 A/h, el cálculo del consumo diario y mensual es el siguiente:

- **Consumo diario**:
  $$Consumo \ diario = 1.5 \ A \times 24 \ h = 36 \ Ah$$

- **Consumo mensual**:
  $$Consumo \ mensual = 36 \ Ah/día \times 30 \ días = 1080 \ Ah$$

## Placa Solar

Para alimentar una Raspberry Pi 4 con un consumo de 1.5 A/h, necesitarás una placa solar que pueda generar suficiente energía. Si consideramos una placa solar de 100 W, y suponiendo que recibes un promedio de 5 horas de sol pico al día, la producción diaria de la placa sería:

$$Producción \ diaria = 100 \ W \times 5 \ h = 500 \ Wh$$

Dado que la Raspberry Pi consume 432 Wh al día (1.5 A a 12 V), una sola placa de 100 W sería suficiente para cubrir el consumo diario, siempre y cuando se utilice un sistema de almacenamiento adecuado (batería).

## Montaje del Sistema Solar

### Componentes necesarios

- Placa solar (100 W)
- Controlador de carga
- Batería 
- Inversor (si la Raspberry Pi requiere corriente alterna)
- Cables y conectores

### Conexión

1. Conecta la placa solar al controlador de carga.
2. Conecta el controlador de carga a la batería.
3. Si es necesario, conecta el inversor a la batería y luego a la Raspberry Pi.

### Precio
- Los precios de los cuales nos tenemos que hacer cargo son:
1. Raspberry Pi Zero 2W 29,90€ (Amazon)
2. Panel Solar 12V 100W Policristalino 83.99€ (Leroy Merlin) 

## Montar un Servidor en Raspberry Pi

Para montar un servidor en tu Raspberry Pi, puedes seguir estos pasos:

### 1. Preparar la Raspberry Pi

- **Instalar el sistema operativo**:
  - Descarga la imagen de Raspberry Pi OS desde el sitio oficial.
  - Usa una herramienta como Balena Etcher para grabar la imagen en una tarjeta microSD.
  - Inserta la tarjeta microSD en la Raspberry Pi y enciéndela.

### 2. Configurar la Raspberry Pi

- **Conectar a la red**:
  - Conéctate a tu red Wi-Fi o usa un cable Ethernet.
  
- **Actualizar el sistema**:
  ```bash
  sudo apt update
  sudo apt upgrade

### 3. Instalar el software del servidor

Dependiendo del tipo de servidor que desees montar, puedes elegir entre varias opciones. Aquí hay algunos ejemplos:

- **Servidor web (Apache)**:
  ```bash
  sudo apt install apache2
- **Servidor de aplicaciones (Node.js)**:
  ```bash
  sudo apt install nodejs npm

- **Servidor de base de datos (MySQL)**:
  ```bash
  sudo apt install mysql-server

### 4. Configurar el servidor
- **Configurar Apache**:
- Coloca tus archivos web en /var/www/html.
- Puedes acceder a tu servidor web desde un navegador ingresando la dirección IP de la Raspberry Pi.
- **Configurar MySQL**:
 Asegúrate de asegurar tu instalación de MySQL:
  ```bash
  sudo mysql_secure_installation
- **Configurar Node.js**:
- Crea tu aplicación y ejecuta el servidor con:
  ```bash
  node app.js
  
### 5. Acceso remoto
- SSH: Habilita SSH para acceder a tu Raspberry Pi de forma remota
```bash
sudo raspi-config

```

# Parte del readme 

# Raspberry Pi y Energía Solar
### Integrantes
Sergio Aragón Garcia

Francisco de Paula Alba Muñoz

Juan Herrador Rello

Abel Suazo Cabeza de Vaca

## Introducción

Este proyecto se centra en la creación de un servidor web alimentado exclusivamente por energía renovable, demostrando que es posible desarrollar soluciones tecnológicas sostenibles y accesibles.

Para ello, se utilizará una Raspberry Pi, un microordenador de bajo consumo energético, como base del servidor. Este dispositivo ofrece una combinación ideal de eficiencia y versatilidad, lo que lo convierte en una opción perfecta para aplicaciones ligeras como un servidor web.

## Selección del Hardware: CPU

### Comparativa de Modelos de Raspberry Pi y Alternativa

| Modelo                  | Consumo Energético (reposo/carga) | Rendimiento (CPU/RAM)       | Ventajas                       | Desventajas                    |
|-------------------------|------------------------------------|-----------------------------|--------------------------------|--------------------------------|
| **Raspberry Pi Zero W** | ~0.5W / ~1.2W                     | 1 núcleo / 512MB RAM        | Muy bajo consumo; económico.   | Rendimiento limitado.          |
| **Raspberry Pi 3B+**    | ~1.2W / ~4W                       | 4 núcleos / 1GB RAM         | Buen balance entre consumo y potencia. | Menor eficiencia que el Pi 4.  |
| **Raspberry Pi 4 (4GB)**| ~3W / ~6W                         | 4 núcleos / hasta 8GB RAM   | Excelente rendimiento; multitarea. | Alto consumo para proyectos solares pequeños. |
| **Raspberry Pi 400**    | ~6W / ~10W                        | 4 núcleos / 4GB RAM         | Integración con teclado; ideal para aprendizaje. | Diseño menos compacto.         |

### Alternativa: ODROID-C4

| Modelo                  | Consumo Energético                | Rendimiento (CPU/RAM)       | Ventajas                       | Desventajas                    |
|-------------------------|------------------------------------|-----------------------------|--------------------------------|--------------------------------|
| **ODROID-C4**           | ~2W / ~4W                         | 4 núcleos / 4GB RAM         | Similar al Raspberry Pi 4 pero más eficiente energéticamente. | Menor soporte de comunidad y software. |

### Conclusiones

Tras analizar las diferentes opciones, hemos obtenido las siguientes conclusiones en relación a las necesidades de este proyecto:

- **Raspberry Pi Zero W**: Es la opción ideal si el tráfico web será bajo (servidor estático) y el presupuesto es reducido. Su bajo consumo la hace perfecta para un sistema alimentado con un panel solar pequeño (~5W).

- **Raspberry Pi 3B+**: Una buena opción para proyectos con requerimientos moderados, como un servidor dinámico con tráfico ocasional. Sin embargo, su consumo energético demanda un panel solar más potente, de aproximadamente 10W.

- **Raspberry Pi 4**: Es la mejor elección si se necesita alto rendimiento (por ejemplo, para bases de datos o aplicaciones más pesadas). No obstante, su mayor consumo energético implica una configuración solar más robusta, con un panel de ~20W o superior.

- **ODROID-C4**: Representa una alternativa eficiente si se busca un rendimiento similar al Raspberry Pi 4, pero con un consumo energético algo menor. A pesar de esto, su menor soporte de comunidad y software podría dificultar su implementación en comparación con las opciones de Raspberry Pi.

## Consumo Diario y Mensual de la Raspberry Pi Zero W

### Suposiciones:
- **Consumo en reposo**: 0.5W
- **Consumo en carga ligera**: 1.2W
- **Horas de funcionamiento por día**: 24 horas
- **Panel solar** de 5W para alimentar el dispositivo

### Cálculo del Consumo Diario

#### Consumo en reposo:
0.5W * 24 horas = **12 Wh/día**

#### Consumo en carga ligera:
1.2W * 24 horas = **28.8 Wh/día**

Por lo tanto, el consumo diario de la Raspberry Pi Zero W varía entre **12 Wh/día** y **28.8 Wh/día**, dependiendo de las condiciones de carga.

### Cálculo del Consumo Mensual

#### Consumo en reposo:
12 Wh/día * 30 días = **360 Wh/mes** o **0.36 kWh/mes**

#### Consumo en carga ligera:
28.8 Wh/día * 30 días = **864 Wh/mes** o **0.864 kWh/mes**

Entonces, el consumo mensual de la Raspberry Pi Zero W puede variar entre **0.36 kWh/mes** y **0.864 kWh/mes**.

**Fuentes:** 

ECO ENERGY GEEK. (s.f.). *Raspberry Pi Zero W power consumption*. Recuperado de https://ecoenergygeek.com  
RASPI.TV. (2018, 6 de marzo). *Power consumption of the Raspberry Pi Zero W*. Recuperado de https://raspi.tv  
RASPBERRY PI SPY. (2019, 10 de abril). *Raspberry Pi Zero W power usage*. Recuperado de https://raspberrypi-spy.co.uk  

## Placa Solar

Para alimentar una Raspberry Pi 4 con un consumo de 1.5 A/h, necesitarás una placa solar que pueda generar suficiente energía. Si consideramos una placa solar de 100 W, y suponiendo que recibes un promedio de 5 horas de sol pico al día, la producción diaria de la placa sería:

$$Producción \ diaria = 100 \ W \times 5 \ h = 500 \ Wh$$

Dado que la Raspberry Pi consume 432 Wh al día (1.5 A a 12 V), una sola placa de 100 W sería suficiente para cubrir el consumo diario, siempre y cuando se utilice un sistema de almacenamiento adecuado (batería).

## Montaje del Sistema Solar

### Componentes necesarios

- Placa solar (100 W)
- Controlador de carga
- Batería 
- Inversor (si la Raspberry Pi requiere corriente alterna)
- Cables y conectores

### Conexión

1. Conecta la placa solar al controlador de carga.
2. Conecta el controlador de carga a la batería.
3. Si es necesario, conecta el inversor a la batería y luego a la Raspberry Pi.

### Precio
- Los precios de los cuales nos tenemos que hacer cargo son:
1. Raspberry Pi Zero 2W 29,90€ (Amazon)
2. Panel Solar 12V 100W Policristalino 83.99€ (Leroy Merlin)
3. Electronicx Bateria Solar AGM 12v 100ah Marine Edition Barcos Barcas Caravanas Autocaravanas Camper Camping Furgos Bateria Solar de Ciclo Profundo 159€ (amazon)
4. Cables 20-30 eruos conectores
5. Accesorios para módulo solar de 20 A, 12 V, 24 V, cable de conexión fotovoltaico con pinza de cocodrilo (conectado a la batería) para conectar el panel solar. 50€ (Amazon)

## Montar un Servidor en Raspberry Pi

Para montar un servidor en tu Raspberry Pi, puedes seguir estos pasos:

### 1. Preparar la Raspberry Pi

- **Instalar el sistema operativo**:
  - Descarga la imagen de Raspberry Pi OS desde el sitio oficial.
  - Usa una herramienta como Balena Etcher para grabar la imagen en una tarjeta microSD.
  - Inserta la tarjeta microSD en la Raspberry Pi y enciéndela.

### 2. Configurar la Raspberry Pi

- **Conectar a la red**:
  - Conéctate a tu red Wi-Fi o usa un cable Ethernet.
  
- **Actualizar el sistema**:
  ```bash
  sudo apt update
  sudo apt upgrade

### 3. Instalar el software del servidor

Dependiendo del tipo de servidor que desees montar, puedes elegir entre varias opciones. Aquí hay algunos ejemplos:

- **Servidor web (Apache)**:
  ```bash
  sudo apt install apache2
- **Servidor de aplicaciones (Node.js)**:
  ```bash
  sudo apt install nodejs npm

- **Servidor de base de datos (MySQL)**:
  ```bash
  sudo apt install mysql-server

### 4. Configurar el servidor
- **Configurar Apache**:
 - Coloca tus archivos web en /var/www/html.
 - Puedes acceder a tu servidor web desde un navegador ingresando la dirección IP de la Raspberry Pi.
- **Configurar MySQL**:
 Asegúrate de asegurar tu instalación de MySQL:
  ```bash
  sudo mysql_secure_installation
- **Configurar Node.js**:
- Crea tu aplicación y ejecuta el servidor con:
  ```bash
  node app.js
  
### 5. Acceso remoto
- SSH: Habilita SSH para acceder a tu Raspberry Pi de forma remota
```bash
sudo raspi-config
```





