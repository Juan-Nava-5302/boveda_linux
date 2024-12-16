El comando `wget` en Linux es una herramienta de línea de comandos utilizada para descargar archivos desde la web. Es parte del proyecto GNU y soporta los protocolos HTTP, HTTPS y FTP. Aquí tienes una guía detallada sobre su uso:

### **Uso Básico**

```bash
wget URL
```

Este comando descarga el archivo especificado por la URL y lo guarda en el directorio actual.

### **Sintaxis**

```bash
wget [opciones] URL
```

- **`URL`**: La dirección del archivo que deseas descargar.
- **`opciones`**: Opciones adicionales que modifican el comportamiento del comando.

### **Opciones Comunes**

1. **`-O`**: Guarda el archivo descargado con un nombre específico.
    
    ```bash
    wget -O nuevo_nombre.txt https://ejemplo.com/archivo.txt
    ```
    
2. **`-P`**: Guarda el archivo descargado en un directorio específico.
    
    ```bash
    wget -P /ruta/del/directorio https://ejemplo.com/archivo.txt
    ```
    
3. **`-c`**: Reanuda una descarga interrumpida.
    
    ```bash
    wget -c https://ejemplo.com/archivo_grande.zip
    ```
    
4. **`-b`**: Descarga el archivo en segundo plano.
    
    ```bash
    wget -b https://ejemplo.com/archivo_grande.zip
    ```
    
5. **`--limit-rate`**: Limita la velocidad de descarga.
    
    ```bash
    wget --limit-rate=500k https://ejemplo.com/archivo_grande.zip
    ```
    
6. **`-r`**: Descarga de manera recursiva, útil para descargar sitios web completos.
    
    ```bash
    wget -r https://ejemplo.com
    ```
    
7. **`--no-check-certificate`**: Omite la verificación del certificado SSL.
    
    ```bash
    wget --no-check-certificate https://ejemplo.com/archivo.zip
    ```
    

### **Ejemplos Prácticos**

- **Descargar un archivo y guardarlo con un nombre específico**:
    
    ```bash
    wget -O nuevo_nombre.txt https://ejemplo.com/archivo.txt
    ```
    
- **Guardar un archivo en un directorio específico**:
    
    ```bash
    wget -P /ruta/del/directorio https://ejemplo.com/archivo.txt
    ```
    
- **Reanudar una descarga interrumpida**:
    
    ```bash
    wget -c https://ejemplo.com/archivo_grande.zip
    ```
    
- **Descargar un archivo en segundo plano**:
    
    ```bash
    wget -b https://ejemplo.com/archivo_grande.zip
    ```
    
- **Limitar la velocidad de descarga a 500 KB/s**:
    
    ```bash
    wget --limit-rate=500k https://ejemplo.com/archivo_grande.zip
    ```
    
- **Descargar un sitio web completo de manera recursiva**:
    
    ```bash
    wget -r https://ejemplo.com
    ```
    

### **Consideraciones Adicionales**

- **Instalación**: En la mayoría de las distribuciones de Linux, `wget` viene preinstalado. Si no está instalado, puedes instalarlo usando el gestor de paquetes de tu distribución:
    
    - **Ubuntu/Debian**:
        
        ```bash
        sudo apt install wget
        ```
        
    - **CentOS/Fedora**:
        
        ```bash
        sudo yum install wget
        ```
        
- **Uso en Scripts**: `wget` es muy útil en scripts para automatizar la descarga de archivos. Por ejemplo, puedes usar `wget` en un script de shell para descargar automáticamente actualizaciones o archivos de configuración.