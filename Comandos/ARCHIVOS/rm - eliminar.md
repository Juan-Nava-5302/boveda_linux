El comando `rm` en Linux se utiliza para eliminar archivos y directorios.

```bash
rm archivo.txt
```

### **Opciones**

1. **`-r` o `--recursive`**: Elimina directorios y su contenido de forma recursiva.
    
    ```bash
    rm -r directorio
    ```
    
2. **`-f` o `--force`**: Fuerza la eliminación sin pedir confirmación, incluso si los archivos están protegidos contra escritura.
    
    ```bash
    rm -f archivo.txt
    ```
    
3. **`-i` o `--interactive`**: Pide confirmación antes de eliminar cada archivo.
    
    ```bash
    rm -i archivo.txt
    ```
    
4. **`-v` o `--verbose`**: Muestra los archivos que se están eliminando.
    
    ```bash
    rm -v archivo.txt
    ```
    
5. **`-d`**: Elimina directorios vacíos.
    
    ```bash
    rm -d directorio_vacio
    ```
