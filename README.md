# sistema-vigilancia
Sistema de vigilancia para casa usando Raspberry y Arduino.



## Dependencias

```bash
sudo apt-get update && sudo apt-get upgrade
```

Instalar `CMake`:

```bash
sudo apt-get install -y build-essential cmake pkg-config
```

A continuación, necesitamos instalar algunos paquetes de E/S de imagen que nos permitan cargar varios formatos de archivo de imagen desde el disco. Ejemplos de estos formatos de archivo incluyen JPEG, PNG, TIFF, etc:

```bash
sudo apt-get install -y libjpeg-dev libtiff5-dev libjasper-dev libpng12-dev
```

Así como necesitamos paquetes de E/S de imagen, también necesitamos paquetes de E/S de vídeo. Estas librerías nos permiten leer varios formatos de archivos de vídeo desde el disco, así como trabajar directamente con secuencias de vídeo:

```bash
sudo apt-get install -y libavcodec-dev libavformat-dev libswscale-dev libv4l-dev
sudo apt-get install -y libxvidcore-dev libx264-dev
```

La librería OpenCV viene con un sub-módulo llamado highgui que se usa para mostrar imágenes a nuestra pantalla y construir GUIs básicas. Para compilar el módulo highgui, necesitamos instalar la librería de desarrollo GTK:

```bash
sudo apt-get install -y libgtk2.0-dev libgtk-3-dev
```

Muchas operaciones dentro de OpenCV (a saber, las operaciones de matriz) pueden optimizarse aún más instalando algunas dependencias adicionales:

```bash
sudo apt-get install -y libatlas-base-dev gfortran
```

Estas bibliotecas de optimización son especialmente importantes para dispositivos con recursos limitados como el Raspberry Pi.

Por último, instalemos los archivos de cabecera de Python 2.7 y Python 3 para que podamos compilar OpenCV con enlaces de Python:

```bash
sudo apt-get install -y python3-dev
```

