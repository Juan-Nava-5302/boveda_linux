El comando `stat` en Linux se utiliza para mostrar información detallada sobre archivos y sistemas de archivos. A continuación, se presenta una guía sobre su uso y las opciones más comunes.

### Sintaxis

```bash
stat [OPCIÓN]... ARCHIVO...
```

### Ejemplo Básico

Para obtener información básica sobre un archivo, simplemente ejecuta:

```bash
stat archivo.txt
```

### Salida del Comando

La salida típica del comando `stat` incluye:

- **File**: Nombre del archivo.
- **Size**: Tamaño del archivo en bytes.
- **Blocks**: Número de bloques asignados.
- **IO Block**: Tamaño del bloque de E/S.
- **File type**: Tipo de archivo (por ejemplo, archivo regular, directorio, enlace simbólico).
- **Device**: Número de dispositivo en hexadecimal y decimal.
- **Inode**: Número de inodo.
- **Links**: Número de enlaces duros.
- **Access**: Permisos del archivo en formato numérico y simbólico.
- **Uid**: ID de usuario y nombre del propietario.
- **Gid**: ID de grupo y nombre del propietario.
- **Access**: Última vez que se accedió al archivo.
- **Modify**: Última vez que se modificó el contenido del archivo.
- **Change**: Última vez que se cambió el atributo o contenido del archivo.
- **Birth**: Tiempo de creación del archivo (no soportado en Linux).

### Opciones Comunes

- **-f, --file-system**: Muestra información sobre el sistema de archivos en lugar del archivo en sí.
- **-L, --dereference**: Sigue enlaces simbólicos y muestra información sobre el archivo al que apuntan.
- **-c, --format**: Personaliza el formato de salida.
- **–printf**: Similar a `--format`, pero permite interpretar secuencias de escape.

### Ejemplos de Uso

1. **Mostrar información detallada de un archivo:**
    
    ```bash
    stat archivo.txt
    ```
    
2. **Mostrar solo el tamaño del archivo:**
    
    ```bash
    stat -c "%s" archivo.txt
    ```
    
3. **Mostrar información del sistema de archivos:**
    
    ```bash
    stat -f archivo.txt
    ```
    
4. **Seguir enlaces simbólicos:**
    
    ```bash
    stat -L enlace_simbolico
    ```
    
5. **Formato personalizado:**
    
    ```bash
    stat --format="%n %s %y" archivo.txt
    ```