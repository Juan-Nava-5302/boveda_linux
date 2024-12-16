El comando `nano` en Linux es un editor de texto simple y fácil de usar, ideal para usuarios que necesitan editar archivos de texto desde la línea de comandos sin la complejidad de editores más avanzados como `vim` o `emacs`. Aquí tienes una guía detallada sobre su uso:

### **Uso Básico**

```bash
nano nombre_del_archivo
```

Este comando abre el archivo especificado en el editor `nano`. Si el archivo no existe, `nano` lo creará.

### **Sintaxis**

```bash
nano [opciones] nombre_del_archivo
```

- **`nombre_del_archivo`**: El archivo que deseas abrir o crear.
- **`opciones`**: Opciones adicionales que modifican el comportamiento del comando.

### **Comandos Básicos en `nano`**

- **Abrir un archivo**:
    
    ```bash
    nano archivo.txt
    ```
    
- **Guardar cambios**: Presiona `Ctrl + O` (escribe el nombre del archivo y presiona Enter).
    
- **Salir del editor**: Presiona `Ctrl + X`.
    
- **Cortar una línea**: Presiona `Ctrl + K`.
    
- **Pegar una línea**: Presiona `Ctrl + U`.
    
- **Copiar una línea**: Presiona `Alt + 6`.
    
- **Buscar texto**: Presiona `Ctrl + W` y escribe el término de búsqueda.
    
- **Reemplazar texto**: Presiona `Ctrl + \` y sigue las instrucciones.
    

### **Opciones Comunes**

1. **`-c`**: Muestra la posición del cursor (línea y columna).
    
    ```bash
    nano -c archivo.txt
    ```
    
2. **`-m`**: Habilita el soporte para el uso del ratón.
    
    ```bash
    nano -m archivo.txt
    ```
    
3. **`-i`**: Indenta automáticamente las nuevas líneas para que coincidan con la indentación de la línea anterior.
    
    ```bash
    nano -i archivo.txt
    ```
    
4. **`-r`**: Ajusta el texto a un ancho específico.
    
    ```bash
    nano -r 80 archivo.txt
    ```
    

### **Atajos de Teclado Útiles**

- **Mostrar ayuda**: `Ctrl + G`
- **Justificar párrafo**: `Ctrl + J`
- **Ir a una línea específica**: `Ctrl + _`
- **Deshacer**: `Alt + U`
- **Rehacer**: `Alt + E`

### **Ejemplos Prácticos**

- **Abrir un archivo y mostrar la posición del cursor**:
    
    ```bash
    nano -c archivo.txt
    ```
    
- **Abrir un archivo con soporte para el ratón**:
    
    ```bash
    nano -m archivo.txt
    ```
    
- **Abrir un archivo y ajustar el texto a 80 caracteres de ancho**:
    
    ```bash
    nano -r 80 archivo.txt
    ```
    

### **Personalización de `nano`**

Puedes personalizar `nano` editando el archivo de configuración `nanorc`, que generalmente se encuentra en `/etc/nanorc` para configuraciones globales o en `~/.nanorc` para configuraciones específicas del usuario. [Aquí puedes habilitar características como el resaltado de sintaxis y la numeración de líneas](https://linuxize.com/post/how-to-use-nano-text-editor/)[1](https://linuxize.com/post/how-to-use-nano-text-editor/)[2](https://www.arsys.es/blog/comandos-nano).