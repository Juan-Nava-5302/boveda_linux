El comando `ip` en Linux es una herramienta poderosa para la configuración y gestión de interfaces de red. Es parte del paquete `iproute2`, que ha reemplazado en gran medida al comando `ifconfig` en muchas distribuciones modernas. Aquí tienes una guía detallada sobre su uso:

### **Uso Básico**

```bash
ip [opciones] objeto {comando | help}
```

- **`objeto`**: El tipo de objeto que deseas gestionar (por ejemplo, `link`, `address`, `route`, `neigh`).
- **`comando`**: La acción que deseas realizar sobre el objeto (por ejemplo, `show`, `add`, `del`).
- **`opciones`**: Opciones adicionales que modifican el comportamiento del comando.

### **Objetos Comunes**

1. **`link`**: Muestra y modifica interfaces de red.
2. **`address`**: Muestra y modifica direcciones IP.
3. **`route`**: Muestra y altera la tabla de enrutamiento.
4. **`neigh`**: Muestra y manipula objetos vecinos (tabla ARP).

### **Comandos Comunes**

1. **Mostrar información sobre interfaces de red**:
    
    ```bash
    ip link show
    ```
    
2. **Mostrar direcciones IP**:
    
    ```bash
    ip addr show
    ```
    
3. **Asignar una dirección IP a una interfaz**:
    
    ```bash
    sudo ip addr add 192.168.1.100/24 dev eth0
    ```
    
4. **Eliminar una dirección IP de una interfaz**:
    
    ```bash
    sudo ip addr del 192.168.1.100/24 dev eth0
    ```
    
5. **Mostrar la tabla de enrutamiento**:
    
    ```bash
    ip route show
    ```
    
6. **Añadir una ruta**:
    
    ```bash
    sudo ip route add 192.168.1.0/24 via 192.168.1.1
    ```
    
7. **Eliminar una ruta**:
    
    ```bash
    sudo ip route del 192.168.1.0/24
    ```
    

### **Ejemplos Prácticos**

- **Mostrar todas las interfaces de red y sus estados**:
    
    ```bash
    ip link show
    ```
    
- **Mostrar todas las direcciones IP asignadas a las interfaces**:
    
    ```bash
    ip addr show
    ```
    
- **Asignar una dirección IP a una interfaz**:
    
    ```bash
    sudo ip addr add 192.168.1.100/24 dev eth0
    ```
    
- **Eliminar una dirección IP de una interfaz**:
    
    ```bash
    sudo ip addr del 192.168.1.100/24 dev eth0
    ```
    
- **Mostrar la tabla de enrutamiento**:
    
    ```bash
    ip route show
    ```
    
- **Añadir una ruta a la tabla de enrutamiento**:
    
    ```bash
    sudo ip route add 192.168.1.0/24 via 192.168.1.1
    ```
    

### **Consideraciones Adicionales**

- **Persistencia**: Las configuraciones realizadas con el comando `ip` no son persistentes y se perderán después de un reinicio. [Para hacerlas permanentes, debes editar los archivos de configuración específicos de tu distribución o agregar los comandos a un script de inicio](https://linuxize.com/post/linux-ip-command/)[1](https://linuxize.com/post/linux-ip-command/).
- **Permisos**: La mayoría de los comandos `ip` requieren permisos de superusuario, por lo que es común usar `sudo`.