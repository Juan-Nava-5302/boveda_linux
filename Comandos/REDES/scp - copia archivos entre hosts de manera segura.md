El comando `scp` (Secure Copy) en Linux se utiliza para copiar archivos y directorios de forma segura entre sistemas locales y remotos utilizando el protocolo SSH. Es una herramienta muy útil para transferir datos de manera segura. Aquí tienes una guía detallada sobre su uso:

### **Uso Básico**

```bash
scp archivo_origen usuario@host_destino:/ruta/destino
```

Este comando copia el `archivo_origen` al `host_destino` en la ruta especificada.

### **Sintaxis**

```bash
scp [opciones] [origen] [destino]
```

- **`origen`**: El archivo o directorio que deseas copiar.
- **`destino`**: La ubicación de destino, que puede ser local o remota.
- **`opciones`**: Opciones adicionales que modifican el comportamiento del comando.

### **Opciones Comunes**

1. **`-r`**: Copia directorios de manera recursiva.
    
    ```bash
    scp -r directorio usuario@host_destino:/ruta/destino
    ```
    
2. **`-P`**: Especifica el puerto SSH.
    
    ```bash
    scp -P 2222 archivo_origen usuario@host_destino:/ruta/destino
    ```
    
3. **`-C`**: Comprime los datos durante la transferencia.
    
    ```bash
    scp -C archivo_origen usuario@host_destino:/ruta/destino
    ```
    
4. **`-i`**: Especifica un archivo de clave privada para la autenticación.
    
    ```bash
    scp -i /ruta/a/clave_privada archivo_origen usuario@host_destino:/ruta/destino
    ```
    
5. **`-v`**: Muestra información detallada sobre el proceso de transferencia.
    
    ```bash
    scp -v archivo_origen usuario@host_destino:/ruta/destino
    ```
    

### **Ejemplos Prácticos**

- **Copiar un archivo a un servidor remoto**:
    
    ```bash
    scp archivo.txt usuario@servidor:/ruta/destino
    ```
    
- **Copiar un archivo desde un servidor remoto a tu máquina local**:
    
    ```bash
    scp usuario@servidor:/ruta/archivo.txt /ruta/local
    ```
    
- **Copiar un directorio completo de manera recursiva**:
    
    ```bash
    scp -r directorio usuario@servidor:/ruta/destino
    ```
    
- **Especificar un puerto SSH diferente**:
    
    ```bash
    scp -P 2222 archivo.txt usuario@servidor:/ruta/destino
    ```
    
- **Usar un archivo de clave privada para la autenticación**:
    
    ```bash
    scp -i ~/.ssh/id_rsa archivo.txt usuario@servidor:/ruta/destino
    ```
    

### **Consideraciones Adicionales**

- [**Seguridad**: `scp` utiliza SSH para la transferencia de datos, lo que garantiza que los datos estén cifrados durante la transmisión](https://www.howtogeek.com/804179/scp-command-linux/)[1](https://www.howtogeek.com/804179/scp-command-linux/)[2](https://www.ionos.es/digitalguide/servidores/configuracion/scp-de-linux/).
- [**Deprecación**: Aunque `scp` sigue siendo ampliamente utilizado, se considera obsoleto en algunas distribuciones modernas y se recomienda usar `rsync` o `sftp` para transferencias más avanzadas](https://www.howtogeek.com/804179/scp-command-linux/)[1](https://www.howtogeek.com/804179/scp-command-linux/)[2](https://www.ionos.es/digitalguide/servidores/configuracion/scp-de-linux/).

[El comando `scp` es una herramienta esencial para la transferencia segura de archivos en Linux, proporcionando una forma sencilla y segura de copiar datos entre sistemas](https://www.howtogeek.com/804179/scp-command-linux/)[1](https://www.howtogeek.com/804179/scp-command-linux/)[2](https://www.ionos.es/digitalguide/servidores/configuracion/scp-de-linux/)[3](https://bing.com/search?q=comando+scp+de+linux).