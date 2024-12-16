El comando `vim` (Vi IMproved) en Linux es un editor de texto avanzado basado en el editor `vi`. Es conocido por su eficiencia y flexibilidad, y es ampliamente utilizado por desarrolladores y administradores de sistemas. Aquí tienes una guía detallada sobre su uso:

### **Uso Básico**

```bash
vim nombre_del_archivo
```

Este comando abre el archivo especificado en el editor `vim`. Si el archivo no existe, `vim` lo creará.

### **Modos de `vim`**

`vim` tiene varios modos, pero los más importantes son:

1. **Modo Comando**: Es el modo predeterminado al iniciar `vim`. Aquí puedes ejecutar comandos para navegar y manipular texto.
2. **Modo Insertar**: Aquí puedes escribir y editar texto. Para entrar en este modo, presiona `i` desde el Modo Comando.
3. **Modo Visual**: Permite seleccionar texto para copiar, cortar o manipular.

### **Comandos Básicos**

- **Entrar en Modo Insertar**: Presiona `i` para insertar texto antes del cursor, o `a` para insertar después del cursor.
- **Guardar y Salir**: Desde el Modo Comando, escribe `:wq` y presiona Enter para guardar y salir. Si solo quieres salir sin guardar, usa `:q!`.
- **Navegación**: Usa las teclas `h`, `j`, `k`, `l` para moverte a la izquierda, abajo, arriba y derecha respectivamente.
- **Eliminar Texto**: Usa `x` para eliminar el carácter bajo el cursor, `dd` para eliminar una línea completa.
- **Copiar y Pegar**: Usa `yy` para copiar una línea y `p` para pegarla después del cursor.

### **Comandos de Movimiento**

- **`gg`**: Mover al principio del archivo.
- **`G`**: Mover al final del archivo.
- **`w`**: Mover al principio de la siguiente palabra.
- **`b`**: Mover al principio de la palabra anterior.
- **`0`**: Mover al principio de la línea actual.
- **`$`**: Mover al final de la línea actual.

### **Comandos de Edición**

- **`u`**: Deshacer el último cambio.
- **`Ctrl + r`**: Rehacer el último cambio deshecho.
- **`dw`**: Eliminar desde el cursor hasta el final de la palabra.
- **`d$`**: Eliminar desde el cursor hasta el final de la línea.
- **`y`**: Copiar (yank) texto.
- **`p`**: Pegar texto copiado.

### **Buscar y Reemplazar**

- **Buscar**: Presiona `/` seguido del término de búsqueda y Enter.
- **Reemplazar**: Usa `:%s/viejo/nuevo/g` para reemplazar todas las ocurrencias de `viejo` con `nuevo` en el archivo.

### **Ejemplos Prácticos**

- **Abrir un archivo**:
    
    ```bash
    vim archivo.txt
    ```
    
- **Guardar y salir**:
    
    ```bash
    :wq
    ```
    
- **Salir sin guardar**:
    
    ```bash
    :q!
    ```
    
- **Copiar una línea**:
    
    ```bash
    yy
    ```
    
- **Pegar una línea**:
    
    ```bash
    p
    ```
    

### **Personalización de `vim`**

Puedes personalizar `vim` editando el archivo de configuración `.vimrc`, que generalmente se encuentra en el directorio personal del usuario. [Aquí puedes habilitar características como el resaltado de sintaxis, la numeración de líneas y más](https://itsfoss.com/es/comandos-basicos-de-vim/)[1](https://itsfoss.com/es/comandos-basicos-de-vim/)[2](https://linuxhandbook.com/basic-vim-commands/).