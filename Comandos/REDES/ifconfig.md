El comando `ifconfig` en Linux se utiliza para configurar y mostrar el estado de las interfaces de red. Es una herramienta esencial para la gestión de redes, aunque en distribuciones modernas ha sido reemplazada en gran medida por el comando `ip`. Aquí tienes una guía detallada sobre su uso:

### **Uso Básico**

```bash
ifconfig
```

Este comando muestra la configuración de todas las interfaces de red activas.

### **Sintaxis**

```bash
ifconfig [opciones] [interfaz]
```

- **`interfaz`**: El nombre de la interfaz de red que deseas configurar o consultar.
- **`opciones`**: Opciones adicionales que modifican el comportamiento del comando.

### **Opciones Comunes**

1. **`-a`**: Muestra la configuración de todas las interfaces, activas e inactivas.
    
    ```bash
    ifconfig -a
    ```
    
2. **`-s`**: Muestra un resumen corto de todas las interfaces.
    
    ```bash
    ifconfig -s
    ```
    
3. **`up`**: Activa una interfaz de red.
    
    ```bash
    ifconfig eth0 up
    ```
    
4. **`down`**: Desactiva una interfaz de red.
    
    ```bash
    ifconfig eth0 down
    ```
    
5. **`inet`**: Asigna una dirección IP a una interfaz.
    
    ```bash
    ifconfig eth0 192.168.1.100
    ```
    
6. **`netmask`**: Configura la máscara de red.
    
    ```bash
    ifconfig eth0 netmask 255.255.255.0
    ```
    
7. **`broadcast`**: Configura la dirección de broadcast.
    
    ```bash
    ifconfig eth0 broadcast 192.168.1.255
    ```
    
8. **`mtu`**: Cambia la Unidad Máxima de Transmisión (MTU).
    
    ```bash
    ifconfig eth0 mtu 1500
    ```
    
9. **`promisc`**: Activa el modo promiscuo, permitiendo que la interfaz capture todos los paquetes.
    
    ```bash
    ifconfig eth0 promisc
    ```
    

### **Ejemplos Prácticos**

- **Mostrar la configuración de todas las interfaces de red**:
    
    ```bash
    ifconfig -a
    ```
    
- **Asignar una dirección IP y máscara de red a una interfaz**:
    
    ```bash
    ifconfig eth0 192.168.1.100 netmask 255.255.255.0
    ```
    
- **Activar una interfaz de red**:
    
    ```bash
    ifconfig eth0 up
    ```
    
- **Desactivar una interfaz de red**:
    
    ```bash
    ifconfig eth0 down
    ```
    
- **Cambiar la dirección MAC de una interfaz**:
    
    ```bash
    ifconfig eth0 hw ether 00:11:22:33:44:55
    ```
    

### **Consideraciones Adicionales**

- [**Deprecación**: `ifconfig` es parte del paquete `net-tools`, que ha sido reemplazado en muchas distribuciones modernas por el comando `ip` debido a su soporte más completo y actualizado para IPv6 y otras características avanzadas](https://linuxize.com/post/ifconfig-command/)[1](https://linuxize.com/post/ifconfig-command/)[2](https://phoenixnap.com/kb/linux-ifconfig).
- **Instalación**: Si `ifconfig` no está disponible en tu sistema, puedes instalarlo con:
    - **Ubuntu/Debian**:
        
        ```bash
        sudo apt install net-tools
        ```
        
    - **CentOS/RHEL**:
        
        ```bash
        sudo yum install net-tools
        ```