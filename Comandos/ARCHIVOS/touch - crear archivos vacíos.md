El comando `touch` en Linux se utiliza principalmente para crear archivos vacíos y para cambiar las marcas de tiempo de los archivos o carpetas.

```bash
touch nombre_del_archivo
```

### **Opciones Comunes**

1. **`-a`**: Cambia solo la marca de tiempo de acceso.
    
    ```bash
    touch -a archivo.txt
    ```
    
2. **`-m`**: Cambia solo la marca de tiempo de modificación.
    
    ```bash
    touch -m archivo.txt
    ```
    
3. **`-c`**: No crea un nuevo archivo si no existe.
    
    ```bash
    touch -c archivo.txt
    ```
    
4. **`-d`**: Establece la fecha y hora usando una cadena de caracteres.
    
    ```bash
    touch -d '2024-10-28 16:31' archivo.txt
    ```
    
5. **`-t`**: Establece la fecha y hora en un formato específico.
    
    ```bash
    touch -t 202410281631.00 archivo.txt
    ```
    
6. **`-r`**: Usa las marcas de tiempo de otro archivo como referencia.
    
    ```bash
    touch -r archivo_referencia.txt archivo.txt
    ```