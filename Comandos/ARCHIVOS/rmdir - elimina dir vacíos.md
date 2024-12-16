El comando `rmdir` en Linux se utiliza para eliminar directorios vacíos.

```bash
rmdir nombre_del_directorio
```

### **Opciones Comunes**

1. **`-p` o `--parents`**: Elimina el directorio especificado y sus directorios padres si están vacíos.
    
    ```bash
    rmdir -p ruta/del/directorio
    ```
    
2. **`-v` o `--verbose`**: Muestra un mensaje por cada directorio eliminado.
    
    ```bash
    rmdir -v nombre_del_directorio
    ```
    
3. **`--ignore-fail-on-non-empty`**: No muestra un mensaje de error si el directorio no está vacío.
    
    ```bash
    rmdir --ignore-fail-on-non-empty nombre_del_directorio
    ```