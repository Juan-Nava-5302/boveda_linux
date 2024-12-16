El comando `uname` en Linux se utiliza para mostrar información sobre el sistema operativo y el kernel. Es una herramienta útil para obtener detalles básicos del sistema. Aquí tienes una guía detallada sobre su uso:

### **Uso Básico**

```bash
uname
```

Este comando muestra el nombre del kernel del sistema operativo.

### **Sintaxis**

```bash
uname [opciones]
```

- **`opciones`**: Opciones adicionales que modifican el comportamiento del comando.

### **Opciones Comunes**

1. **`-a`**: Muestra toda la información disponible.
    
    ```bash
    uname -a
    ```
    
    Salida típica:
    
    ```bash
    Linux hostname 5.4.0-42-generic #46-Ubuntu SMP Fri Jul 10 00:24:02 UTC 2020 x86_64 x86_64 x86_64 GNU/Linux
    ```
    
2. **`-s`**: Muestra el nombre del kernel.
    
    ```bash
    uname -s
    ```
    
    Salida:
    
    ```bash
    Linux
    ```
    
3. **`-n`**: Muestra el nombre del host del sistema.
    
    ```bash
    uname -n
    ```
    
    Salida:
    
    ```bash
    hostname
    ```
    
4. **`-r`**: Muestra la versión del kernel.
    
    ```bash
    uname -r
    ```
    
    Salida:
    
    ```bash
    5.4.0-42-generic
    ```
    
5. **`-v`**: Muestra la versión del kernel.
    
    ```bash
    uname -v
    ```
    
    Salida:
    
    ```bash
    #46-Ubuntu SMP Fri Jul 10 00:24:02 UTC 2020
    ```
    
6. **`-m`**: Muestra la arquitectura del hardware.
    
    ```bash
    uname -m
    ```
    
    Salida:
    
    ```bash
    x86_64
    ```
    
7. **`-p`**: Muestra el tipo de procesador.
    
    ```bash
    uname -p
    ```
    
    Salida:
    
    ```bash
    x86_64
    ```
    
8. **`-i`**: Muestra la plataforma de hardware.
    
    ```bash
    uname -i
    ```
    
    Salida:
    
    ```bash
    x86_64
    ```
    
9. **`-o`**: Muestra el nombre del sistema operativo.
    
    ```bash
    uname -o
    ```
    
    Salida:
    
    ```bash
    GNU/Linux
    ```
    

### **Ejemplos Prácticos**

- **Mostrar toda la información del sistema**:
    
    ```bash
    uname -a
    ```
    
- **Mostrar solo el nombre del kernel**:
    
    ```bash
    uname -s
    ```
    
- **Mostrar la versión del kernel**:
    
    ```bash
    uname -r
    ```
    
- **Mostrar la arquitectura del hardware**:
    
    ```bash
    uname -m
    ```
    

### **Consideraciones Adicionales**

- [**Compatibilidad**: El comando `uname` es compatible con la mayoría de las distribuciones de Linux y es una herramienta estándar para obtener información del sistema](https://linuxenespanol.net/uso-del-comando-uname-con-ejemplos/)[1](https://linuxenespanol.net/uso-del-comando-uname-con-ejemplos/)[2](https://linuxhandbook.com/uname/)[3](https://bing.com/search?q=comando+uname+de+linux).