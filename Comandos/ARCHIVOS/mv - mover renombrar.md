El comando `mv` en Linux se utiliza para mover y renombrar archivos y directorios.

Este comando mueve el archivo `archivo_origen` a `archivo_destino`. Si `archivo_destino` es un directorio, el archivo se moverá dentro de ese directorio.

### **Parámetros** 
 1. _mv -i archivo_origen archivo_destino_ : Pide confirmación antes de sobrescribir archivos existentes.
 2. _mv -f archivo_origen archivo_destino_ :  Fuerza la operación sin pedir confirmación, incluso si el archivo de destino está protegido contra escritura
 3. _mv -n archivo_origen archivo_destino_ : No sobrescribe archivos existentes en el destino.
 4. _mv -v archivo_origen archivo_destino_ : Muestra los archivos que se están moviendo.
 5. _mv -u archivo_origen archivo_destino_ : Solo mueve los archivos si el archivo de origen es más reciente que el archivo de destino o si el archivo de destino no existe.

### Sintaxis

```bash
mv [OPCIÓN]... ORIGEN... DESTINO
```

### Ejemplos Básicos

1. **Mover un archivo a otro directorio**:
    
    ```bash
    mv archivo.txt /ruta/al/directorio/
    ```
    
    Este comando moverá `archivo.txt` al directorio especificado.
    
2. **Renombrar un archivo**:
    
    ```bash
    mv archivo_viejo.txt archivo_nuevo.txt
    ```
    
    Este comando renombrará `archivo_viejo.txt` a `archivo_nuevo.txt`.
    
3. **Mover múltiples archivos a un directorio**:
    
    ```bash
    mv archivo1.txt archivo2.txt /ruta/al/directorio/
    ```
    
    Este comando moverá `archivo1.txt` y `archivo2.txt` al directorio especificado.
    

### Opciones Comunes

- **-i, --interactive**: Solicita confirmación antes de sobrescribir.
    
    ```bash
    mv -i archivo.txt /ruta/al/directorio/
    ```
    
- **-f, --force**: No solicita confirmación antes de sobrescribir.
    
    ```bash
    mv -f archivo.txt /ruta/al/directorio/
    ```
    
- **-n, --no-clobber**: No sobrescribe archivos existentes.
    
    ```bash
    mv -n archivo.txt /ruta/al/directorio/
    ```
    
- **-v, --verbose**: Muestra los archivos a medida que se mueven.
    
    ```bash
    mv -v archivo.txt /ruta/al/directorio/
    ```
    

### Ejemplos Avanzados

1. **Mover un directorio**:
    
    ```bash
    mv /ruta/al/directorio_origen /ruta/al/directorio_destino
    ```
    
2. **Renombrar un directorio**:
    
    ```bash
    mv /ruta/al/directorio_viejo /ruta/al/directorio_nuevo
    ```
    
3. **Mover archivos con un patrón específico**:
    
    ```bash
    mv *.txt /ruta/al/directorio/
    ```
    
    Este comando moverá todos los archivos con extensión `.txt` al directorio especificado.
    

### Consideraciones

- **Permisos**: Necesitas permisos de escritura en el directorio de origen y en el de destino.
- **Sobrescritura**: Por defecto, `mv` sobrescribe archivos sin preguntar. Usa las opciones `-i` o `-n` para cambiar este comportamiento.