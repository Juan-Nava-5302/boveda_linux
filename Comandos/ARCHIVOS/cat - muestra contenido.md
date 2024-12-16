El comando `cat` en Linux, abreviatura de “concatenate” (concatenar), es una herramienta fundamental para la manipulación y visualización de archivos de texto.

```bash
cat nombre_del_archivo
```

### **Opciones Comunes**

1. **`-n`**: Muestra los números de línea junto con el contenido del archivo.
    
    ```bash
    cat -n archivo.txt
    ```
    
2. **`-b`**: Muestra los números de línea solo para las líneas no vacías.
    
    ```bash
    cat -b archivo.txt
    ```
    
3. **`-s`**: Suprime las líneas vacías repetidas.
    
    ```bash
    cat -s archivo.txt
    ```
    
4. **`-E`**: Muestra un símbolo `$` al final de cada línea.
    
    ```bash
    cat -E archivo.txt
    ```
    
5. **`-T`**: Muestra los caracteres de tabulación como `^I`.
    
    ```bash
    cat -T archivo.txt
    ```

# PRUEBAS

![[{cat}.png]]