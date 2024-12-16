El comando `whereis` en Linux se utiliza para localizar los archivos binarios, de origen y las páginas de manual de un comando específico. Es una herramienta útil para encontrar rápidamente la ubicación de estos archivos esenciales en el sistema. Aquí tienes una guía detallada sobre su uso:

### **Uso Básico**

```bash
whereis comando
```

Este comando muestra las ubicaciones del archivo binario, el archivo fuente y la página de manual del comando especificado.

### **Sintaxis**

```bash
whereis [opciones] comando
```

- **`comando`**: El nombre del comando del que deseas obtener información.
- **`opciones`**: Opciones adicionales que modifican el comportamiento del comando.

### **Opciones Comunes**

1. **`-b`**: Muestra solo los archivos binarios.
    
    ```bash
    whereis -b comando
    ```
    
2. **`-m`**: Muestra solo las páginas de manual.
    
    ```bash
    whereis -m comando
    ```
    
3. **`-s`**: Muestra solo los archivos fuente.
    
    ```bash
    whereis -s comando
    ```
    
4. **`-B`**: Busca archivos binarios en directorios específicos.
    
    ```bash
    whereis -B /ruta/a/directorio -f comando
    ```
    
5. **`-M`**: Busca páginas de manual en directorios específicos.
    
    ```bash
    whereis -M /ruta/a/directorio -f comando
    ```
    
6. **`-S`**: Busca archivos fuente en directorios específicos.
    
    ```bash
    whereis -S /ruta/a/directorio -f comando
    ```
    
7. **`-u`**: Busca entradas inusuales que no tengan exactamente un archivo binario, una página de manual y un archivo fuente.
    
    ```bash
    whereis -u comando
    ```
    

### **Ejemplos Prácticos**

- **Encontrar la ubicación del comando `ls`**:
    
    ```bash
    whereis ls
    ```
    
    Salida típica:
    
    ```bash
    ls: /bin/ls /usr/share/man/man1/ls.1.gz
    ```
    
- **Mostrar solo los archivos binarios del comando `ls`**:
    
    ```bash
    whereis -b ls
    ```
    
- **Mostrar solo las páginas de manual del comando `ls`**:
    
    ```bash
    whereis -m ls
    ```
    
- **Buscar archivos binarios en un directorio específico**:
    
    ```bash
    whereis -B /bin -f ls
    ```
    

### **Consideraciones Adicionales**

- [**Compatibilidad**: El comando `whereis` es compatible con la mayoría de las distribuciones de Linux y es una herramienta estándar para localizar archivos relacionados con comandos](https://phoenixnap.com/kb/whereis-command-linux)[1](https://phoenixnap.com/kb/whereis-command-linux)[2](https://linuxize.com/post/whereis-command-in-linux/)[3](https://bing.com/search?q=comando+whereis+de+linux).