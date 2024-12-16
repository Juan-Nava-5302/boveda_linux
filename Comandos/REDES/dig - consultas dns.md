El comando `dig` (Domain Information Groper) en Linux es una herramienta poderosa para realizar consultas en el sistema de nombres de dominio (DNS). Es ampliamente utilizado por administradores de sistemas y desarrolladores para obtener información detallada sobre registros DNS. Aquí tienes una guía detallada sobre su uso:

### **Uso Básico**

```bash
dig dominio
```

Este comando realiza una consulta DNS para el dominio especificado y devuelve el registro A (dirección IP) por defecto.

### **Sintaxis**

```bash
dig [servidor] [nombre] [tipo]
```

- **`servidor`**: Opcional, la dirección IP o el nombre del servidor DNS a consultar. Si no se especifica, `dig` utilizará los servidores DNS configurados en `/etc/resolv.conf`.
- **`nombre`**: El dominio o nombre de recurso que deseas consultar.
- **`tipo`**: El tipo de registro DNS a consultar (por ejemplo, A, MX, SOA). Si no se indica, `dig` realiza una búsqueda del tipo A por defecto.

### **Opciones Comunes**

1. **`+short`**: Muestra solo la respuesta corta.
    
    ```bash
    dig ejemplo.com +short
    ```
    
2. **`+noall +answer`**: Muestra solo la sección de respuestas.
    
    ```bash
    dig ejemplo.com +noall +answer
    ```
    
3. **`@servidor`**: Especifica un servidor DNS diferente para la consulta.
    
    ```bash
    dig @8.8.8.8 ejemplo.com
    ```
    
4. **`ANY`**: Consulta todos los tipos de registros DNS disponibles para un dominio.
    
    ```bash
    dig ejemplo.com ANY
    ```
    
5. **`MX`**: Consulta los registros de intercambio de correo (Mail Exchange).
    
    ```bash
    dig ejemplo.com MX
    ```
    
6. **`TXT`**: Consulta los registros de texto.
    
    ```bash
    dig ejemplo.com TXT
    ```
    
7. **`+trace`**: Rastrea el camino de las consultas DNS desde la raíz hasta el servidor final.
    
    ```bash
    dig ejemplo.com +trace
    ```
    
8. **`-x`**: Realiza una búsqueda inversa de DNS para encontrar el nombre de dominio asociado a una dirección IP.
    
    ```bash
    dig -x 192.168.1.1
    ```
    

### **Ejemplos Prácticos**

- **Consultar un dominio y obtener solo la IP**:
    
    ```bash
    dig ejemplo.com +short
    ```
    
- **Consultar un dominio usando el servidor DNS de Google**:
    
    ```bash
    dig @8.8.8.8 ejemplo.com
    ```
    
- **Consultar todos los registros DNS de un dominio**:
    
    ```bash
    dig ejemplo.com ANY
    ```
    
- **Consultar los registros MX de un dominio**:
    
    ```bash
    dig ejemplo.com MX
    ```
    
- **Realizar una búsqueda inversa de DNS**:
    
    ```bash
    dig -x 8.8.8.8
    ```
    

### **Instalación**

El comando `dig` forma parte del paquete `dnsutils` en Debian/Ubuntu y `bind-utils` en CentOS/Fedora. Puedes instalarlo usando el gestor de paquetes de tu distribución:

- **Ubuntu/Debian**:
    
    ```bash
    sudo apt install dnsutils
    ```
    
- **CentOS/Fedora**:
    
    ```bash
    sudo yum install bind-utils
    ```