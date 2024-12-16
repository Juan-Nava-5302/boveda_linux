El comando `fg` en Linux se utiliza para traer trabajos en segundo plano al primer plano. Es una herramienta útil para la gestión de trabajos en la línea de comandos, permitiendo que los procesos que se están ejecutando en segundo plano vuelvan a la terminal activa. Aquí tienes una guía detallada sobre su uso:

### **Uso Básico**

```bash
fg [job_spec]
```

Este comando trae el trabajo especificado por `job_spec` al primer plano.

### **Sintaxis**

```bash
fg [opciones] [job_spec]
```

- **`job_spec`**: La especificación del trabajo que deseas traer al primer plano. Puede ser el número del trabajo, un prefijo del nombre del comando, o un símbolo de porcentaje seguido del número del trabajo (por ejemplo, `%1`).
- **`opciones`**: Opciones adicionales que modifican el comportamiento del comando.

### **Ejemplos Prácticos**

- **Listar trabajos actuales**:
    
    ```bash
    jobs
    ```
    
    Esto muestra una lista de trabajos actuales con sus números de trabajo.
    
- **Suspender un trabajo en ejecución**: Mientras un comando está en ejecución, presiona `Ctrl + Z` para suspenderlo.
    
- **Reanudar el trabajo más reciente en primer plano**:
    
    ```bash
    fg
    ```
    
- **Reanudar un trabajo específico en primer plano**:
    
    ```bash
    fg %1
    ```
    
    Donde `%1` es el número del trabajo que deseas traer al primer plano.
    

### **Uso Combinado con Otros Comandos**

- **Ejecutar un comando en segundo plano desde el inicio**: Puedes ejecutar un comando directamente en segundo plano añadiendo `&` al final del comando:
    
    ```bash
    comando &
    ```
    
- **Mover un trabajo en segundo plano**: Usa el comando `bg` para mover un trabajo suspendido al segundo plano:
    
    ```bash
    bg %1
    ```
    

### **Consideraciones Adicionales**

- **Gestión de Trabajos**: El comando `fg` es parte de un conjunto de comandos para la gestión de trabajos en la línea de comandos, incluyendo `jobs` para listar trabajos y `bg` para reanudar trabajos en segundo plano.
- **Uso en Scripts**: Aunque `fg` es útil en la línea de comandos interactiva, su uso en scripts es menos común, ya que los scripts suelen manejar procesos en segundo plano de manera diferente.