El comando `cal` en Linux es una herramienta útil para visualizar calendarios directamente desde la terminal. Aquí tienes una guía detallada sobre su uso:

### **Uso Básico**

```bash
cal
```

Este comando muestra el calendario del mes actual.

### **Sintaxis**

```bash
cal [opciones] [[día] mes] año
```

- **`día`**: Opcional, el día específico a resaltar.
- **`mes`**: El mes que deseas mostrar (1-12).
- **`año`**: El año que deseas mostrar (debe ser especificado completamente, por ejemplo, 2024).
- **`opciones`**: Opciones adicionales que modifican el comportamiento del comando.

### **Opciones Comunes**

1. **`-1`**: Muestra solo el mes actual (comportamiento predeterminado).
    
    ```bash
    cal -1
    ```
    
2. **`-3`**: Muestra el mes anterior, el actual y el siguiente.
    
    ```bash
    cal -3
    ```
    
3. **`-y`**: Muestra el calendario completo del año actual.
    
    ```bash
    cal -y
    ```
    
4. **`-m`**: Muestra el calendario del mes especificado.
    
    ```bash
    cal -m 5
    ```
    
5. **`-j`**: Muestra los días del año (números julianos).
    
    ```bash
    cal -j
    ```
    
6. **`-s`**: Muestra el domingo como el primer día de la semana.
    
    ```bash
    cal -s
    ```
    
7. **`-n`**: Muestra un número específico de meses a partir del mes actual.
    
    ```bash
    cal -n 3
    ```
    
8. **`-d`**: Muestra el calendario de un mes y año específicos.
    
    ```bash
    cal -d 2024-06
    ```
    

### **Ejemplos Prácticos**

- **Mostrar el calendario del mes actual**:
    
    ```bash
    cal
    ```
    
- **Mostrar el calendario del año completo**:
    
    ```bash
    cal -y
    ```
    
- **Mostrar el calendario de un mes específico**:
    
    ```bash
    cal 5 2024
    ```
    
- **Mostrar el calendario con días julianos**:
    
    ```bash
    cal -j
    ```
    
- **Mostrar el calendario del mes actual y los dos meses siguientes**:
    
    ```bash
    cal -3
    ```
    

### **Consideraciones Adicionales**

- [**Compatibilidad**: El comando `cal` es parte del paquete `util-linux`, que está disponible en la mayoría de las distribuciones de Linux](https://adictec.com/como-usar-comando-cal-linux/)[1](https://adictec.com/como-usar-comando-cal-linux/)[2](https://www.man7.org/linux/man-pages/man1/cal.1.html).
- **Uso en Scripts**: `cal` es útil en scripts para generar calendarios y planificar tareas.
# PRUEBAS 

![[cal.png]]