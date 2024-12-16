El comando `cp` en Linux se utiliza para copiar archivos y directorios de una ubicación a otra.

```bash
cp [opciones] archivo_origen archivo_destino
```

### Parámetros

1. _cp -r directorio_origen directorio_destino_ :  Copia directorios de forma recursiva, incluyendo todos los subdirectorios y archivos.
2. _cp -i archivo_origen archivo_destino_ : Pide confirmación antes de sobrescribir archivos existentes.
3. _cp -u archivo_origen archivo_destino_ : Copia solo si el archivo de origen es más reciente que el archivo de destino o si el archivo de destino no existe.
4. _cp -v archivo_origen archivo_destino_ : Muestra los archivos que se están copiando.
5. _cp -a directorio_origen directorio_destino_  : Copia archivos y directorios, preservando la estructura, permisos, y metadatos.
6.  _cp -p archivo_origen archivo_destino_ : Preserva los atributos del archivo original, como los permisos y las marcas de tiempo.
7. _cp -b archivo.txt /ruta/destino/_ : Crear una copia de seguridad antes de sobrescribir.
8. _cp -u archivo.txt /ruta/destino/_ : Copiar solo si el archivo de destino es más antiguo.