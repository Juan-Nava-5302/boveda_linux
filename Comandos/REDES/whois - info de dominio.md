El comando `whois` en Linux se utiliza para obtener información sobre la propiedad y el registro de nombres de dominio y direcciones IP. Es una herramienta útil para consultar bases de datos que contienen detalles sobre los dominios registrados y sus propietarios. Aquí tienes una guía detallada sobre su uso:

### **Uso Básico**

```bash
whois dominio_o_direccion_ip
```

Este comando muestra la información WHOIS asociada con el dominio o la dirección IP especificada.

### **Sintaxis**

```bash
whois [opciones] objeto
```

- **`objeto`**: El nombre de dominio o la dirección IP que deseas consultar.
- **`opciones`**: Opciones adicionales que modifican el comportamiento del comando.

### **Opciones Comunes**

1. **`-h HOST`**: Especifica el servidor WHOIS a consultar.
    
    ```bash
    whois -h whois.verisign-grs.com dominio.com
    ```
    
2. **`-p PUERTO`**: Especifica el puerto de red para la conexión.
    
    ```bash
    whois -p 43 dominio.com
    ```
    
3. **`--verbose`**: Muestra detalles completos de la consulta.
    
    ```bash
    whois --verbose dominio.com
    ```
    
4. **`--help`**: Muestra la ayuda del comando.
    
    ```bash
    whois --help
    ```
    

### **Ejemplos Prácticos**

- **Consultar información WHOIS de un dominio**:
    
    ```bash
    whois google.com
    ```
    
- **Consultar información WHOIS de una dirección IP**:
    
    ```bash
    whois 8.8.8.8
    ```
    
- **Especificar un servidor WHOIS diferente**:
    
    ```bash
    whois -h whois.arin.net google.com
    ```
    

### **Información Típica de WHOIS**

La información devuelta por una consulta WHOIS puede incluir:

- **Nombre del dominio**: El nombre del dominio consultado.
- **ID del registro**: Identificador único del dominio en el registro.
- **Servidor WHOIS del registrador**: El servidor WHOIS del registrador del dominio.
- **URL del registrador**: La URL del registrador del dominio.
- **Fecha de creación**: La fecha en que el dominio fue registrado.
- **Fecha de expiración**: La fecha en que el registro del dominio expira.
- **Estado del dominio**: El estado actual del dominio (por ejemplo, activo, en espera de eliminación).
- **Información del registrante**: Nombre y contacto del propietario del dominio.
- **Información del administrador**: Nombre y contacto del administrador del dominio.
- **Información técnica**: Nombre y contacto del responsable técnico del dominio.
- [**Servidores de nombres**: Los servidores DNS asociados con el dominio](https://www.howtogeek.com/680086/how-to-use-the-whois-command-on-linux/)[1](https://www.howtogeek.com/680086/how-to-use-the-whois-command-on-linux/)[2](https://www.solvetic.com/tutoriales/article/8799-como-utilizar-comando-whois-linux-para-que-sirve-usar-e-instalar/).

### **Instalación**

El comando `whois` no siempre está instalado por defecto en todas las distribuciones de Linux. Puedes instalarlo usando el gestor de paquetes de tu distribución:

- **Ubuntu/Debian**:
    
    ```bash
    sudo apt install whois
    ```
    
- **CentOS/Fedora**:
    
    ```bash
    sudo dnf install whois
    ```