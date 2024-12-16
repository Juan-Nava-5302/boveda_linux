El comando `whoami` en Linux es una herramienta sencilla pero útil que muestra el nombre del usuario actualmente conectado al sistema. Aquí tienes una guía detallada sobre su uso:

### **Uso Básico**

```bash
whoami
```

Este comando muestra el nombre del usuario efectivo en la sesión actual de la terminal.

### **Sintaxis**

```bash
whoami [opciones]
```

- **`opciones`**: Opciones adicionales que modifican el comportamiento del comando.

### **Opciones Comunes**

1. **`--help`**: Muestra un mensaje de ayuda y sale.
    
    ```bash
    whoami --help
    ```
    
2. **`--version`**: Muestra la versión del comando `whoami` y sale.
    
    ```bash
    whoami --version
    ```
    

### **Ejemplos Prácticos**

- **Mostrar el nombre del usuario actual**:
    
    ```bash
    whoami
    ```
    
    Salida típica:
    
    ```bash
    usuario
    ```
    
- **Verificar el usuario efectivo después de cambiar de usuario**:
    
    ```bash
    su otro_usuario
    whoami
    ```
    
    Esto mostrará `otro_usuario` si el cambio de usuario fue exitoso.
    
- **Comprobar si un usuario tiene privilegios de sudo**:
    
    ```bash
    sudo whoami
    ```
    
    Si tienes privilegios de sudo, la salida será `root`.
    

### **Uso en Scripts**

El comando `whoami` es útil en scripts para verificar qué usuario está ejecutando el script. Por ejemplo, puedes usarlo para asegurarte de que un script se está ejecutando como root:

```bash
if [[ "$(whoami)" != "root" ]]; then
  echo "Este script debe ejecutarse como root."
  exit 1
fi
```

### **Comparación con Otros Comandos**

- **`who`**: Muestra una lista de todos los usuarios actualmente conectados al sistema.
- **`id`**: Muestra información detallada sobre el usuario, incluyendo el ID de usuario, el ID de grupo y los grupos a los que pertenece.
- [**`logname`**: Muestra el nombre de inicio de sesión del usuario actual](https://phoenixnap.com/kb/whoami-linux)[1](https://phoenixnap.com/kb/whoami-linux)[2](https://bing.com/search?q=comando+whoami+de+linux)[3](https://ioflood.com/blog/whoami-linux-command/).