El comando `df` en Linux se utiliza para mostrar información sobre el uso del espacio en disco de los sistemas de archivos montados. Es una herramienta esencial para monitorear y gestionar el espacio en disco. Aquí tienes una guía detallada sobre su uso:

### **Uso Básico**

```bash
df
```

Este comando muestra información sobre todos los sistemas de archivos montados, incluyendo el tamaño total, el espacio utilizado, el espacio disponible y el punto de montaje.

### **Sintaxis**

```bash
df [opciones] [archivo...]
```

- **`archivo`**: El archivo o sistema de archivos del que deseas obtener información.
- **`opciones`**: Opciones adicionales que modifican el comportamiento del comando.

### **Opciones Comunes**

1. **`-h`**: Muestra los tamaños en un formato legible para humanos (KB, MB, GB).
    
    ```bash
    df -h
    ```
    
2. **`-a`**: Incluye todos los sistemas de archivos, incluso los que tienen un tamaño de 0 bloques.
    
    ```bash
    df -a
    ```
    
3. **`-T`**: Muestra el tipo de sistema de archivos.
    
    ```bash
    df -T
    ```
    
4. **`-i`**: Muestra el uso de inodos en lugar del uso de bloques.
    
    ```bash
    df -i
    ```
    
5. **`-t`**: Muestra solo los sistemas de archivos de un tipo específico.
    
    ```bash
    df -t ext4
    ```
    
6. **`-x`**: Excluye los sistemas de archivos de un tipo específico.
    
    ```bash
    df -x tmpfs
    ```
    
7. **`--total`**: Muestra un total general al final de la salida.
    
    ```bash
    df --total
    ```
    

### **Ejemplos Prácticos**

- **Mostrar el uso del disco en un formato legible para humanos**:
    
    ```bash
    df -h
    ```
    
- **Mostrar el uso del disco incluyendo todos los sistemas de archivos**:
    
    ```bash
    df -a
    ```
    
- **Mostrar el tipo de sistema de archivos**:
    
    ```bash
    df -T
    ```
    
- **Mostrar el uso de inodos**:
    
    ```bash
    df -i
    ```
    
- **Mostrar solo los sistemas de archivos de tipo ext4**:
    
    ```bash
    df -t ext4
    ```
    
- **Excluir los sistemas de archivos de tipo tmpfs**:
    
    ```bash
    df -x tmpfs
    ```
    

### **Interpretación de la Salida**

La salida del comando `df` incluye varias columnas:

- **Filesystem**: El nombre del sistema de archivos.
- **1K-blocks**: El tamaño del sistema de archivos en bloques de 1K.
- **Used**: El espacio utilizado en bloques de 1K.
- **Available**: El espacio disponible en bloques de 1K.
- **Use%**: El porcentaje de espacio utilizado.
- **Mounted on**: El punto de montaje del sistema de archivos.

### **Uso en Scripts**

El comando `df` es muy útil en scripts para monitorear el uso del disco y generar informes. Por ejemplo, puedes usar `df` para verificar si hay suficiente espacio en disco antes de realizar una copia de seguridad:

```bash
#!/bin/bash
espacio_disponible=$(df -h / | grep '/' | awk '{print $4}')
echo "Espacio disponible en /: $espacio_disponible"
```