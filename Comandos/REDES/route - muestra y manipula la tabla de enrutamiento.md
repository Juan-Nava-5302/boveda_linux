El comando `route` en Linux se utiliza para mostrar y manipular la tabla de enrutamiento IP del kernel. Es una herramienta útil para configurar rutas estáticas a hosts o redes específicas a través de una interfaz. Aunque en muchas distribuciones modernas ha sido reemplazado por el comando `ip`, `route` sigue siendo relevante en ciertos contextos. Aquí tienes una guía detallada sobre su uso:

### **Uso Básico**

```bash
route
```

Este comando muestra la tabla de enrutamiento actual.

### **Sintaxis**

```bash
route [opciones] [comando]
```

- **`opciones`**: Opciones adicionales que modifican el comportamiento del comando.
- **`comando`**: La acción que deseas realizar sobre la tabla de enrutamiento (por ejemplo, `add`, `del`).

### **Opciones Comunes**

1. **`-n`**: Muestra las direcciones IP y las máscaras de red en formato numérico, sin resolver nombres de host.
    
    ```bash
    route -n
    ```
    
2. **`add`**: Añade una nueva ruta a la tabla de enrutamiento.
    
    ```bash
    sudo route add -net 192.168.1.0 netmask 255.255.255.0 gw 192.168.1.1
    ```
    
3. **`del`**: Elimina una ruta de la tabla de enrutamiento.
    
    ```bash
    sudo route del -net 192.168.1.0 netmask 255.255.255.0
    ```
    

### **Ejemplos Prácticos**

- **Mostrar la tabla de enrutamiento actual**:
    
    ```bash
    route -n
    ```
    
- **Añadir una ruta estática**:
    
    ```bash
    sudo route add -net 10.0.0.0 netmask 255.255.255.0 gw 192.168.1.1
    ```
    
    Este comando añade una ruta a la red `10.0.0.0/24` a través de la puerta de enlace `192.168.1.1`.
    
- **Eliminar una ruta estática**:
    
    ```bash
    sudo route del -net 10.0.0.0 netmask 255.255.255.0
    ```
    
    Este comando elimina la ruta a la red `10.0.0.0/24`.
    

### **Consideraciones Adicionales**

- **Persistencia**: Las rutas añadidas con el comando `route` no son persistentes y se perderán después de un reinicio. [Para hacerlas permanentes, debes editar los archivos de configuración de red específicos de tu distribución](https://www.cyberciti.biz/faq/linux-route-add/)[1](https://www.cyberciti.biz/faq/linux-route-add/)[2](https://commandmasters.com/commands/route-common/).
- [**Deprecación**: En muchas distribuciones modernas, el comando `route` ha sido reemplazado por el comando `ip` debido a su soporte más completo y actualizado para IPv6 y otras características avanzadas](https://www.cyberciti.biz/faq/linux-route-add/)[3](https://www.certificacaolinux.com.br/comando-linux-route/).

### **Alternativa con el Comando `ip`**

El comando `ip` proporciona funcionalidades similares y es el recomendado en distribuciones modernas:

- **Mostrar la tabla de enrutamiento**:
    
    ```bash
    ip route show
    ```
    
- **Añadir una ruta estática**:
    
    ```bash
    sudo ip route add 10.0.0.0/24 via 192.168.1.1
    ```
    
- **Eliminar una ruta estática**:
    
    ```bash
    sudo ip route del 10.0.0.0/24
    ```
    

[El comando `route` es una herramienta útil para la gestión de rutas en Linux, aunque su uso está siendo reemplazado por el comando `ip` en sistemas modernos](https://www.cyberciti.biz/faq/linux-route-add/)[1](https://www.cyberciti.biz/faq/linux-route-add/)[2](https://commandmasters.com/commands/route-common/)[3](https://www.certificacaolinux.com.br/comando-linux-route/).

¿Hay algo más en lo que pueda ayudarte?

[](https://www.cyberciti.biz/faq/linux-route-add/)[1](https://www.cyberciti.biz/faq/linux-route-add/):  [](https://www.cyberciti.biz/faq/linux-route-add/)[2](https://commandmasters.com/commands/route-common/):  [](https://www.cyberciti.biz/faq/linux-route-add/)[3](https://www.certificacaolinux.com.br/comando-linux-route/): 

[1![](blob:https://outlook.office.com/2e4a9cd1-f104-411f-ab7c-fd0e12a86dd1)cyberciti.biz](https://www.cyberciti.biz/faq/linux-route-add/)[2![](blob:https://outlook.office.com/e6049e4e-007e-4414-9cff-9d09953dc16b)commandmasters.com](https://commandmasters.com/commands/route-common/)[3![](blob:https://outlook.office.com/1d11ec91-4094-453d-9030-274d651c5b5c)certificacaolinux.com.br](https://www.certificacaolinux.com.br/comando-linux-route/)

###### Sent by Copilot:

El comando `route` en Linux se utiliza para mostrar y manipular la tabla de enrutamiento IP del kernel. Es una herramienta útil para configurar rutas estáticas a hosts o redes específicas a través de una interfaz. Aunque en muchas distribuciones modernas ha sido reemplazado por el comando `ip`, `route` sigue siendo relevante en ciertos contextos. Aquí tienes una guía detallada sobre su uso:

### **Uso Básico**

```bash
route
```

Este comando muestra la tabla de enrutamiento actual.

### **Sintaxis**

```bash
route [opciones] [comando]
```

- **`opciones`**: Opciones adicionales que modifican el comportamiento del comando.
- **`comando`**: La acción que deseas realizar sobre la tabla de enrutamiento (por ejemplo, `add`, `del`).

### **Opciones Comunes**

1. **`-n`**: Muestra las direcciones IP y las máscaras de red en formato numérico, sin resolver nombres de host.
    
    ```bash
    route -n
    ```
    
2. **`add`**: Añade una nueva ruta a la tabla de enrutamiento.
    
    ```bash
    sudo route add -net 192.168.1.0 netmask 255.255.255.0 gw 192.168.1.1
    ```
    
3. **`del`**: Elimina una ruta de la tabla de enrutamiento.
    
    ```bash
    sudo route del -net 192.168.1.0 netmask 255.255.255.0
    ```
    

### **Ejemplos Prácticos**

- **Mostrar la tabla de enrutamiento actual**:
    
    ```bash
    route -n
    ```
    
- **Añadir una ruta estática**:
    
    ```bash
    sudo route add -net 10.0.0.0 netmask 255.255.255.0 gw 192.168.1.1
    ```
    
    Este comando añade una ruta a la red `10.0.0.0/24` a través de la puerta de enlace `192.168.1.1`.
    
- **Eliminar una ruta estática**:
    
    ```bash
    sudo route del -net 10.0.0.0 netmask 255.255.255.0
    ```
    
    Este comando elimina la ruta a la red `10.0.0.0/24`.
    

### **Consideraciones Adicionales**

- **Persistencia**: Las rutas añadidas con el comando `route` no son persistentes y se perderán después de un reinicio. Para hacerlas permanentes, debes editar los archivos de configuración de red específicos de tu distribución.
- **Deprecación**: En muchas distribuciones modernas, el comando `route` ha sido reemplazado por el comando `ip` debido a su soporte más completo y actualizado para IPv6 y otras características avanzadas.

### **Alternativa con el Comando `ip`**

El comando `ip` proporciona funcionalidades similares y es el recomendado en distribuciones modernas:

- **Mostrar la tabla de enrutamiento**:
    
    ```bash
    ip route show
    ```
    
- **Añadir una ruta estática**:
    
    ```bash
    sudo ip route add 10.0.0.0/24 via 192.168.1.1
    ```
    
- **Eliminar una ruta estática**:
    
    ```bash
    sudo ip route del 10.0.0.0/24
    ```
    

El comando `route` es una herramienta útil para la gestión de rutas en Linux, aunque su uso está siendo reemplazado por el comando `ip` en sistemas modernos.