# Montaje del Servidor

## Requisitos Previos

- **Raspberry Pi 4** con Raspbian (o Raspberry Pi OS) instalado.
- Conexión a Internet.
- Acceso a la terminal (puedes usar SSH o un monitor y teclado conectados a la Raspberry Pi).

## Pasos para Instalar Apache 2

1. **Actualizar el Sistema**:
   Abre la terminal y ejecuta los siguientes comandos para asegurarte de que tu sistema esté actualizado:

   ```bash
   sudo apt update
   sudo apt upgrade
   ```

2. **Instalar Apache 2**
```bash
  sudo apt install apache2 -y
```

3.**Host interno**
Obtener IP de la Raspberry:
```bash
sudo hostname -I
```
Abrir en navegador: http://<tu_ip> para tener el url del sitio en local

4. **Introducir la pagina web**
   introducimos en nuestro caso la carpeta de nuestro servidor copiandola al directorio html de apache siguiendo los siguietes pasos:
 
   4.1 ** Vamos a la carpeta \html**
     ```bash
      sudo cd /var/www/html
     ```

   4.2 ** Copiamos la carpeta**
   ```bash
    sudo cp -r /var/www/html/mi_carpeta /var/www/html/copia_de_mi_carpeta
   ```

   y ya estaria pasada la carpeta en la cual nosotros hemos pasado los documentos

  
5.**Configuramos permisos**

``` bash 
sudo chown -R www-data:www-data /var/www/html/mi_web
sudo chmod -R 755 /var/www/html/mi_web
```
 en mi web ponemos la carpeta la cual tenga la ruta del index.html

6.**Reiniciamos apache**

   ```bash
    sudo systemctl restart apache2
   ```

7.**Ultimos retoques**

  Para que el servidor se abra cada vez que se encienda la Raspberry ponemos este comando:
  ```bash
  sudo systemctl restart apache2
  ```

Inicio -> **[Volver al inicio ](README.md)**  
Anterior -> **[Placa Solar](placaSolar.md)**  
Siguiente -> **[Presupuesto](precio.md)**
