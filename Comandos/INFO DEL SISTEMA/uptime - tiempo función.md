El comando `uptime` en Linux se utiliza para mostrar cuánto tiempo ha estado en funcionamiento el sistema desde su último reinicio. También proporciona información sobre el número de usuarios conectados y la carga promedio del sistema. Aquí tienes una guía detallada sobre su uso:

### **Uso Básico**

```bash
uptime
```

Este comando muestra la hora actual, el tiempo que el sistema ha estado en funcionamiento, el número de usuarios conectados y la carga promedio del sistema.

### **Sintaxis**

```bash
uptime [opciones]
```

- **`opciones`**: Opciones adicionales que modifican el comportamiento del comando.

### **Salida del Comando**

La salida típica del comando `uptime` se ve así:

```bash
16:13:00 up 2 days, 8:18, 1 user, load average: 1.19, 1.54, 1.51
```

- **16:13:00**: La hora actual del sistema.
- **up 2 days, 8:18**: El tiempo que el sistema ha estado en funcionamiento (2 días, 8 horas y 18 minutos).
- **1 user**: El número de usuarios actualmente conectados al sistema.
- [**load average: 1.19, 1.54, 1.51**: La carga promedio del sistema en los últimos 1, 5 y 15 minutos](https://linuxhandbook.com/uptime-command/)[1](https://linuxhandbook.com/uptime-command/)[2](https://linuxize.com/post/linux-uptime-command/).

### **Opciones Comunes**

1. **`-p`**: Muestra el tiempo de actividad en un formato legible.
    
    ```bash
    uptime -p
    ```
    
    Salida:
    
    ```bash
    up 2 days, 8 hours, 47 minutes
    ```
    
2. **`-s`**: Muestra la fecha y hora desde que el sistema está en funcionamiento.
    
    ```bash
    uptime -s
    ```
    
    Salida:
    
    ```bash
    2024-10-28 07:54:21
    ```
    
3. **`-V`**: Muestra la versión del comando `uptime`.
    
    ```bash
    uptime -V
    ```
    
4. **`-h`**: Muestra la página de ayuda del comando.
    
    ```bash
    uptime -h
    ```
    

### **Ejemplos Prácticos**

- **Mostrar el tiempo de actividad en un formato legible**:
    
    ```bash
    uptime -p
    ```
    
- **Mostrar la fecha y hora desde que el sistema está en funcionamiento**:
    
    ```bash
    uptime -s
    ```
    
### **Consideraciones Adicionales**

- **Carga Promedio**: La carga promedio es una medida de la cantidad de trabajo que el sistema está realizando. Un valor de carga promedio de 1.0 en un sistema de un solo núcleo significa que el sistema está completamente ocupado. [En sistemas con múltiples núcleos, un valor de 1.0 por núcleo indica una carga completa](https://linuxhandbook.com/uptime-command/)[1](https://linuxhandbook.com/uptime-command/)[2](https://linuxize.com/post/linux-uptime-command/).

# PRUEBAS 

El comando `uptime` muestra cuánto tiempo ha estado funcionando el sistema desde su último reinicio, el número de usuarios actualmente conectados y la carga promedio del sistema.

![[{uptime}.png]]