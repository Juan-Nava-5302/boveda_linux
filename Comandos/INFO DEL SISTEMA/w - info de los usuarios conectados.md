El comando `w` en Linux se utiliza para mostrar información sobre los usuarios que están actualmente conectados al sistema y lo que cada usuario está haciendo. También proporciona información sobre cuánto tiempo ha estado funcionando el sistema, la hora actual y la carga promedio del sistema. Aquí tienes una guía detallada sobre su uso:

### **Uso Básico**

```bash
w
```

Este comando muestra una lista de los usuarios conectados y sus actividades actuales.

### **Sintaxis**

```bash
w [opciones] [usuario]
```

- **`usuario`**: Opcional, muestra información solo sobre el usuario especificado.
- **`opciones`**: Opciones adicionales que modifican el comportamiento del comando.

### **Salida del Comando**

La salida típica del comando `w` se ve así:

```bash
16:13:00 up 2 days, 8:18, 1 user, load average: 1.19, 1.54, 1.51
USER     TTY      FROM             LOGIN@   IDLE   JCPU   PCPU WHAT
root     pts/0    192.168.1.100    15:00    1:00   0.02s  0.01s bash
```

- **16:13:00**: La hora actual del sistema.
- **up 2 days, 8:18**: El tiempo que el sistema ha estado en funcionamiento.
- **1 user**: El número de usuarios actualmente conectados.
- **load average: 1.19, 1.54, 1.51**: La carga promedio del sistema en los últimos 1, 5 y 15 minutos.
- **USER**: El nombre del usuario conectado.
- **TTY**: El terminal desde el que el usuario está conectado.
- **FROM**: La dirección IP o el nombre del host desde donde el usuario está conectado.
- **LOGIN@**: La hora en que el usuario inició sesión.
- **IDLE**: El tiempo que el usuario ha estado inactivo.
- **JCPU**: El tiempo de CPU utilizado por todos los procesos asociados al terminal del usuario.
- **PCPU**: El tiempo de CPU utilizado por el proceso actual del usuario.
- [**WHAT**: El comando que el usuario está ejecutando actualmente](https://linuxize.com/post/w-command-in-linux/)[1](https://linuxize.com/post/w-command-in-linux/)[2](https://phoenixnap.com/kb/w-command-in-linux).

### **Opciones Comunes**

1. **`-h`**: No muestra la cabecera.
    
    ```bash
    w -h
    ```
    
2. **`-s`**: Muestra una salida en formato corto.
    
    ```bash
    w -s
    ```
    
3. **`-f`**: Muestra u oculta el campo `FROM`.
    
    ```bash
    w -f
    ```
    
4. **`-i`**: Muestra la dirección IP en lugar del nombre del host en el campo `FROM`.
    
    ```bash
    w -i
    ```
    
5. **`-V`**: Muestra la versión del comando `w`.
    
    ```bash
    w -V
    ```
    

### **Ejemplos Prácticos**

- **Mostrar información sobre todos los usuarios conectados**:
    
    ```bash
    w
    ```
    
- **Mostrar información en un formato corto**:
    
    ```bash
    w -s
    ```
    
- **Mostrar información sin la cabecera**:
    
    ```bash
    w -h
    ```
    
- **Mostrar la dirección IP en lugar del nombre del host**:
    
    ```bash
    w -i
    ```
    

### **Consideraciones Adicionales**

- **Carga Promedio**: La carga promedio es una medida de la cantidad de trabajo que el sistema está realizando. Un valor de carga promedio de 1.0 en un sistema de un solo núcleo significa que el sistema está completamente ocupado. [En sistemas con múltiples núcleos, un valor de 1.0 por núcleo indica una carga completa](https://linuxize.com/post/w-command-in-linux/)[1](https://linuxize.com/post/w-command-in-linux/)[2](https://phoenixnap.com/kb/w-command-in-linux).