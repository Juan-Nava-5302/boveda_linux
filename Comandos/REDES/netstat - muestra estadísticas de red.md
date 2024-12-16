El comando `netstat` en Linux es una herramienta de línea de comandos que proporciona información sobre las conexiones de red, las tablas de enrutamiento, las estadísticas de las interfaces y más. Es muy útil para diagnosticar problemas de red y monitorear la actividad de la red. Aquí tienes una guía detallada sobre su uso:

### **Uso Básico**

```bash
netstat
```

Este comando muestra una lista de todas las conexiones de red activas y las interfaces de red.

### **Sintaxis**

```bash
netstat [opciones]
```

- **`opciones`**: Opciones adicionales que modifican el comportamiento del comando.

### **Opciones Comunes**

1. **`-a`**: Muestra todas las conexiones y puertos de escucha.
    
    ```bash
    netstat -a
    ```
    
2. **`-t`**: Muestra solo las conexiones TCP.
    
    ```bash
    netstat -t
    ```
    
3. **`-u`**: Muestra solo las conexiones UDP.
    
    ```bash
    netstat -u
    ```
    
4. **`-l`**: Muestra solo los puertos en estado de escucha.
    
    ```bash
    netstat -l
    ```
    
5. **`-p`**: Muestra el PID y el nombre del programa que está utilizando cada conexión.
    
    ```bash
    sudo netstat -p
    ```
    
6. **`-n`**: Muestra las direcciones y números de puerto en formato numérico.
    
    ```bash
    netstat -n
    ```
    
7. **`-r`**: Muestra la tabla de enrutamiento del kernel.
    
    ```bash
    netstat -r
    ```
    
8. **`-i`**: Muestra una lista de las interfaces de red y sus estadísticas.
    
    ```bash
    netstat -i
    ```
    
9. **`-s`**: Muestra estadísticas de los protocolos de red.
    
    ```bash
    netstat -s
    ```
    

### **Ejemplos Prácticos**

- **Mostrar todas las conexiones y puertos de escucha**:
    
    ```bash
    netstat -a
    ```
    
- **Mostrar solo las conexiones TCP**:
    
    ```bash
    netstat -t
    ```
    
- **Mostrar solo las conexiones UDP**:
    
    ```bash
    netstat -u
    ```
    
- **Mostrar los puertos en estado de escucha**:
    
    ```bash
    netstat -l
    ```
    
- **Mostrar el PID y el nombre del programa que está utilizando cada conexión**:
    
    ```bash
    sudo netstat -p
    ```
    
- **Mostrar la tabla de enrutamiento del kernel**:
    
    ```bash
    netstat -r
    ```
    
- **Mostrar estadísticas de los protocolos de red**:
    
    ```bash
    netstat -s
    ```
    

### **Interpretación de la Salida**

La salida del comando `netstat` incluye varias columnas importantes:

- **Proto**: El protocolo utilizado (TCP, UDP).
- **Recv-Q**: La cola de recepción de bytes recibidos y listos para ser leídos.
- **Send-Q**: La cola de envío de bytes listos para ser enviados.
- **Local Address**: La dirección y puerto locales.
- **Foreign Address**: La dirección y puerto remotos.
- **State**: El estado de la conexión (por ejemplo, ESTABLISHED, LISTENING).

### **Consideraciones Adicionales**

- [**Deprecación**: Aunque `netstat` sigue siendo ampliamente utilizado, se considera obsoleto en algunas distribuciones modernas y se recomienda usar el comando `ss` como una alternativa más rápida y sencilla](https://www.howtogeek.com/513003/how-to-use-netstat-on-linux/)[1](https://www.howtogeek.com/513003/how-to-use-netstat-on-linux/)[2](https://phoenixnap.com/kb/netstat-command).
- **Permisos**: Algunas opciones de `netstat` requieren permisos de superusuario, por lo que es común usar `sudo`.