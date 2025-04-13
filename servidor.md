# Montaje del Servidor

En nuestro proyecto, el montaje del servidor fue una de las etapas clave para desplegar nuestra página web sostenible en la **Raspberry Pi 4**. A continuación, explicamos los pasos que seguimos para instalar y configurar el servidor web Apache 2.

## Requisitos Previos

Antes de comenzar con el montaje del servidor, nos aseguramos de tener lo siguiente:

- **Raspberry Pi 4** con Raspbian (o Raspberry Pi OS) instalado.
- Conexión a Internet para poder instalar los paquetes necesarios.
- Acceso a la terminal, que en nuestro caso utilizamos a través de SSH, aunque también podríamos haber conectado un monitor y teclado directamente a la Raspberry Pi.

## Pasos para Instalar Apache 2

1. **Actualizar el Sistema**:
   Lo primero que hicimos fue asegurarnos de que el sistema operativo de la Raspberry Pi estuviera completamente actualizado. Para ello, ejecutamos los siguientes comandos en la terminal:

```bash
sudo apt update
sudo apt upgrade
```

2. **Instalar Apache 2**:
A continuación, instalamos Apache 2, que es el servidor web que usamos para alojar nuestra página. Para hacerlo, ejecutamos el siguiente comando:

```bash
  sudo apt install apache2 -y
```


3. **Host Interno**:
Para probar que todo funcionaba correctamente, obtuvimos la dirección IP de nuestra Raspberry Pi con el siguiente comando:

```bash
sudo hostname -I
```

Luego, abrimos un navegador web y escribimos `http://<tu_ip>` para acceder al sitio en local y verificar que el servidor estaba funcionando correctamente.

4. **Introducir la Página Web**:
En nuestro caso, la carpeta que contiene los archivos de la página web se copió al directorio **/var/www/html** de Apache para que se pudiera servir correctamente. Para hacerlo, seguimos estos pasos:

4.1 **Accedemos al directorio HTML**:

```bash
sudo cd /var/www/html
```

4.2 **Copiamos la carpeta de la página web**:
```bash
sudo cp -r /var/www/html/mi_carpeta /var/www/html/copia_de_mi_carpeta
```

Con este paso, copiamos la carpeta que contiene los archivos de nuestro sitio web al directorio adecuado en el servidor.

5. **Configuramos Permisos**:
Para asegurar que el servidor pueda acceder y gestionar los archivos correctamente, ajustamos los permisos de la carpeta de nuestra web. Esto lo hicimos con los siguientes comandos:

``` bash 
sudo chown -R www-data:www-data /var/www/html/mi_web
sudo chmod -R 755 /var/www/html/mi_web
```
Donde `mi_web` es la carpeta que contiene el archivo `index.html`.

6. **Reiniciamos Apache**:
Para asegurarnos de que los cambios fueran aplicados correctamente, reiniciamos el servicio de Apache con el siguiente comando:

```bash
 sudo systemctl restart apache2
```

7. **Últimos retoques**:
Finalmente, configuramos Apache para que se reiniciara automáticamente cada vez que arrancáramos la Raspberry Pi. Esto lo hicimos ejecutando el siguiente comando:

```bash
sudo systemctl restart apache2
```

⬅️ **[Volver al inicio](README.md)**  
⬅️ **[Ir a Consumo Energético](consumo.md)**  
➡️ **[Ir a Presupuesto](precio.md)**
