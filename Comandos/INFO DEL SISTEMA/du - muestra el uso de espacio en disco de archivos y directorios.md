El comando `du` (disk usage) en Linux se utiliza para estimar el uso de espacio en disco de archivos y directorios. Es una herramienta muy útil para identificar qué archivos o carpetas están ocupando más espacio en tu sistema. Aquí tienes una guía detallada sobre su uso:

### **Uso Básico**

```bash
du nombre_del_directorio
```

Este comando muestra el tamaño de todos los archivos y subdirectorios dentro de `nombre_del_directorio`.

### **Sintaxis**

```bash
du [opciones] [ruta]
```

- **`ruta`**: El directorio o archivo del que deseas obtener información.
- **`opciones`**: Opciones adicionales que modifican el comportamiento del comando.

### **Opciones Comunes**

1. **`-h`**: Muestra los tamaños en un formato legible para humanos (KB, MB, GB).
    
    ```bash
    du -h nombre_del_directorio
    ```
    
2. **`-s`**: Muestra solo el total del tamaño del directorio especificado.
    
    ```bash
    du -sh nombre_del_directorio
    ```
    
3. **`-a`**: Muestra el tamaño de todos los archivos, no solo de los directorios.
    
    ```bash
    du -ah nombre_del_directorio
    ```
    
4. **`-c`**: Muestra un total general al final de la salida.
    
    ```bash
    du -ch nombre_del_directorio
    ```
    
5. **`-d`**: Limita la profundidad de la búsqueda a un número específico de niveles.
    
    ```bash
    du -h -d 1 nombre_del_directorio
    ```
    
6. **`--max-depth`**: Similar a `-d`, limita la profundidad de la búsqueda.
    
    ```bash
    du --max-depth=1 nombre_del_directorio
    ```
    
7. **`--exclude`**: Excluye archivos que coincidan con un patrón específico.
    
    ```bash
    du -h --exclude="*.log" nombre_del_directorio
    ```
    

### **Ejemplos Prácticos**

- **Mostrar el tamaño de un directorio en un formato legible para humanos**:
    
    ```bash
    du -h /home/usuario
    ```
    
- **Mostrar solo el tamaño total de un directorio**:
    
    ```bash
    du -sh /home/usuario
    ```
    
- **Mostrar el tamaño de todos los archivos y subdirectorios**:
    
    ```bash
    du -ah /home/usuario
    ```
    
- **Mostrar el tamaño de los directorios hasta una profundidad de 1 nivel**:
    
    ```bash
    du -h --max-depth=1 /home/usuario
    ```
    
- **Mostrar el tamaño total de varios directorios y un total general**:
    
    ```bash
    du -ch /home/usuario /var/log
    ```
    

### **Uso en Scripts**

El comando `du` es muy útil en scripts para monitorear el uso del disco y generar informes. Por ejemplo, puedes usar `du` para encontrar los directorios más grandes en tu sistema:

```bash
du -sh /* | sort -rh | head -10
```

Este comando muestra los 10 directorios más grandes en el sistema raíz.