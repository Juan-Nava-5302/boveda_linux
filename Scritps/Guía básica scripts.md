## 1. Crear el archivo

Con algún editor de texto, crear un archivo cuyo nombre siga la siguiente sitaxis:

nombre_script.sh

## 2. Escribir Script

Depende mucho del tipo de shell o intérprete que estés usando, pues varían en las funciones/lenguajes que soportan.

La estructura básica de un script es la siguiente:

1. **Shebang**: Indica el intérprete que se usará para ejecutar el script.
    
    ```sh
    #!/bin/bash
    ```
    
2. **Comentarios**: Explican partes del script y no se ejecutan.
    
    ```sh
    # Este es un comentario
    ```
    
3. **Variables**: Almacenan valores que se pueden usar más adelante. Por convención usar mayúscula.
    
    ```sh
    NOMBRE="Mundo"
    ```
    
4. **Estructuras de control**: Incluyen condicionales y bucles.
    
    ```sh
    # Condicional
    if [ "$NOMBRE" == "Mundo" ]; then
        echo "Hola, $NOMBRE!"
    fi
    
    # Bucle
    for i in {1..5}; do
        echo "Número $i"
    done
    ```
    
5. **Funciones**: Agrupan comandos que se pueden reutilizar.
    
    ```sh
    mi_funcion() {
        echo "Esta es una función"
    }
    
    mi_funcion
    ```
    
6. **Comandos**: Ejecutan acciones específicas.
    
    ```sh
    echo "Este es un script básico de Linux"
    ```
    

Aquí tienes un ejemplo completo:

```sh
#!/bin/bash

# Este es un script básico de Linux

# Definir una variable
NOMBRE="Mundo"

# Función para saludar
saludar() {
    echo "Hola, $NOMBRE!"
}

# Llamar a la función
saludar

# Bucle para imprimir números
for i in {1..5}; do
    echo "Número $i"
done
```
## 3. Permisos

Otorgar permisos con:

chmod 775 nombre_script.sh

## 4. Ejecutar 

- **Usando la ruta relativa o absoluta**:
    
    ```sh
    ./mi_script.sh
    ```
    
- **Usando `bash` o `sh`**:
    
    ```sh
    bash mi_script.sh
    ```
    
    o
    
    ```sh
    sh mi_script.sh
    ```