El comando `rpm` (Red Hat Package Manager) en Linux se utiliza para gestionar paquetes en sistemas basados en RPM, como RHEL, CentOS y Fedora. La opción `-Uvh` se utiliza específicamente para actualizar o instalar un paquete RPM, mostrando detalles del progreso. Aquí tienes una guía detallada sobre su uso:

### **Uso Básico**

```bash
sudo rpm -Uvh paquete.rpm
```

Este comando actualiza el paquete especificado si ya está instalado o lo instala si no lo está.

### **Sintaxis**

```bash
rpm [opciones] paquete.rpm
```

- **`paquete.rpm`**: El archivo RPM que deseas instalar o actualizar.
- **`opciones`**: Opciones adicionales que modifican el comportamiento del comando.

### **Opciones Comunes**

1. **`-U`**: Actualiza un paquete si ya está instalado o lo instala si no lo está.
    
    ```bash
    sudo rpm -U paquete.rpm
    ```
    
2. **`-v`**: Muestra información detallada durante la instalación o actualización.
    
    ```bash
    sudo rpm -Uv paquete.rpm
    ```
    
3. **`-h`**: Muestra una barra de progreso durante la instalación o actualización.
    
    ```bash
    sudo rpm -Uvh paquete.rpm
    ```
    

### **Ejemplos Prácticos**

- **Actualizar o instalar un paquete RPM con detalles y barra de progreso**:
    
    ```bash
    sudo rpm -Uvh paquete.rpm
    ```
    
- **Instalar un paquete RPM sin actualizar versiones anteriores**:
    
    ```bash
    sudo rpm -ivh paquete.rpm
    ```
    
- **Eliminar un paquete RPM**:
    
    ```bash
    sudo rpm -e nombre_paquete
    ```
    

### **Solución de Problemas Comunes**

- **Dependencias no satisfechas**: Si al instalar o actualizar un paquete con `rpm -Uvh` encuentras errores de dependencias, puedes resolverlas utilizando el comando `yum` o `dnf`:
    
    ```bash
    sudo yum install -y paquete.rpm
    ```
    
    o
    
    ```bash
    sudo dnf install -y paquete.rpm
    ```
    

### **Consideraciones Adicionales**

- **Permisos de Superusuario**: La mayoría de las operaciones con `rpm` requieren permisos de superusuario, por lo que se suelen ejecutar con `sudo`.
- [**Compatibilidad**: `rpm` es específico para sistemas basados en RPM y no funciona en distribuciones basadas en DEB como Debian o Ubuntu](https://www.golinuxcloud.com/rpm-command-in-linux/)[1](https://www.golinuxcloud.com/rpm-command-in-linux/)[2](https://www.tecmint.com/linux-package-management/).