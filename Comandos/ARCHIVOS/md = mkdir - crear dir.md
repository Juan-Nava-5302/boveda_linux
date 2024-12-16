El comando `mkdir` en Linux se utiliza para crear nuevos directorios.

```bash
mkdir nombre_del_directorio
```

### **Parámetros** 
1. **`-p` o `--parents`**: Crea directorios de forma recursiva, incluyendo todos los directorios padres necesarios.
    
    ```bash
    mkdir -p ruta/del/nuevo/directorio
    ```
    ```bash
mkdir -p proyecto/{src,bin,docs}
```

Esto creará la siguiente estructura:

```
proyecto/
├── bin
├── docs
└── src
```

2. **`-m` o `--mode`**: Establece los permisos del nuevo directorio.
    
    ```bash
    mkdir -m 755 nombre_del_directorio
    ```
    
3. **`-v` o `--verbose`**: Muestra un mensaje por cada directorio creado.
    
    ```bash
    mkdir -v nombre_del_directorio
    ```
