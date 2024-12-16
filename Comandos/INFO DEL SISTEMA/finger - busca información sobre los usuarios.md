El comando `finger` en Linux es una herramienta de búsqueda de información sobre los usuarios del sistema. Proporciona detalles como el nombre de inicio de sesión, el nombre real, el terminal, el tiempo de inactividad, la hora de inicio de sesión, la ubicación de la oficina y el número de teléfono de la oficina. Aquí tienes una guía detallada sobre su uso:

### **Uso Básico**

```bash
finger
```

Este comando muestra información sobre todos los usuarios actualmente conectados al sistema.

### **Sintaxis**

```bash
finger [opciones] [usuario]
```

- **`usuario`**: Opcional, muestra información sobre un usuario específico.
- **`opciones`**: Opciones adicionales que modifican el comportamiento del comando.

### **Opciones Comunes**

1. **`-l`**: Muestra la información en un formato largo.
    
    ```bash
    finger -l
    ```
    
2. **`-m`**: No coincide con el nombre completo del usuario.
    
    ```bash
    finger -m usuario
    ```
    
3. **`-p`**: No muestra el contenido de los archivos `.plan`, `.project` y `.pgpkey`.
    
    ```bash
    finger -p usuario
    ```
    
4. **`-s`**: Muestra la información en un formato corto.
    
    ```bash
    finger -s usuario
    ```
    

### **Ejemplos Prácticos**

- **Mostrar información sobre todos los usuarios conectados**:
    
    ```bash
    finger
    ```
    
- **Mostrar información detallada sobre un usuario específico**:
    
    ```bash
    finger usuario
    ```
    
- **Mostrar información en un formato largo**:
    
    ```bash
    finger -l usuario
    ```
    
- **No mostrar el contenido de los archivos `.plan` y `.project`**:
    
    ```bash
    finger -p usuario
    ```
    

### **Instalación**

El comando `finger` no suele estar instalado por defecto en muchas distribuciones de Linux. Puedes instalarlo usando el gestor de paquetes de tu distribución:

- **Ubuntu/Debian**:
    
    ```bash
    sudo apt install finger
    ```
    
- **CentOS/Fedora**:
    
    ```bash
    sudo yum install finger
    ```
    

### **Consideraciones Adicionales**

- [**Archivos `.plan` y `.project`**: Los usuarios pueden crear archivos `.plan` y `.project` en su directorio personal para proporcionar información adicional que se mostrará cuando se ejecute el comando `finger`](https://www.golinuxcloud.com/finger-command-in-linux/)[1](https://www.golinuxcloud.com/finger-command-in-linux/)[2](https://www.howtogeek.com/440391/how-to-use-the-finger-command-on-linux/)[3](https://ioflood.com/blog/finger-linux-command/).