El comando `free` en Linux se utiliza para mostrar información sobre el uso de la memoria del sistema, incluyendo la memoria física (RAM) y la memoria de intercambio (swap). Es una herramienta esencial para monitorear y gestionar el uso de la memoria. Aquí tienes una guía detallada sobre su uso:

### **Uso Básico**

```bash
free
```

Este comando muestra un resumen del uso de la memoria en el sistema.

### **Sintaxis**

```bash
free [opciones]
```

- **`opciones`**: Opciones adicionales que modifican el comportamiento del comando.

### **Salida del Comando**

La salida típica del comando `free` se ve así:

```bash
              total        used        free      shared  buff/cache   available
Mem:        16384256     1234567      234567       12345     4567890     7890123
Swap:        8388608      123456     8265152
```

- **total**: La cantidad total de memoria física o swap.
- **used**: La cantidad de memoria utilizada.
- **free**: La cantidad de memoria libre.
- **shared**: La memoria utilizada por el sistema de archivos tmpfs.
- **buff/cache**: La memoria utilizada por los buffers y la caché.
- [**available**: Una estimación de la memoria disponible para nuevos procesos](https://www.howtogeek.com/456943/how-to-use-the-free-command-on-linux/)[1](https://www.howtogeek.com/456943/how-to-use-the-free-command-on-linux/)[2](https://itsfoss.com/free-command/).

### **Opciones Comunes**

1. **`-h`**: Muestra la información en un formato legible para humanos (KB, MB, GB).
    
    ```bash
    free -h
    ```
    
2. **`-s`**: Actualiza la salida cada `n` segundos.
    
    ```bash
    free -s 5
    ```
    
3. **`-t`**: Muestra una línea con el total de la memoria física y swap.
    
    ```bash
    free -t
    ```
    
4. **`-m`**: Muestra la información en megabytes.
    
    ```bash
    free -m
    ```
    
5. **`-g`**: Muestra la información en gigabytes.
    
    ```bash
    free -g
    ```
    
6. **`-c`**: Muestra la información `n` veces.
    
    ```bash
    free -c 3
    ```
    

### **Ejemplos Prácticos**

- **Mostrar la información de la memoria en un formato legible para humanos**:
    
    ```bash
    free -h
    ```
    
- **Actualizar la salida cada 5 segundos**:
    
    ```bash
    free -s 5
    ```
    
- **Mostrar la información en megabytes**:
    
    ```bash
    free -m
    ```
    
- **Mostrar la información en gigabytes**:
    
    ```bash
    free -g
    ```
    
- **Mostrar la información de la memoria 3 veces**:
    
    ```bash
    free -c 3
    ```
    

### **Consideraciones Adicionales**

- [**Memoria Disponible**: La columna “available” es una estimación de la memoria que está disponible para nuevos procesos sin necesidad de usar swap](https://www.howtogeek.com/456943/how-to-use-the-free-command-on-linux/)[1](https://www.howtogeek.com/456943/how-to-use-the-free-command-on-linux/)[2](https://itsfoss.com/free-command/).
- [**Compatibilidad**: El comando `free` es parte del paquete `procps-ng`, que está disponible en la mayoría de las distribuciones de Linux](https://www.howtogeek.com/456943/how-to-use-the-free-command-on-linux/)[1](https://www.howtogeek.com/456943/how-to-use-the-free-command-on-linux/)[2](https://itsfoss.com/free-command/).