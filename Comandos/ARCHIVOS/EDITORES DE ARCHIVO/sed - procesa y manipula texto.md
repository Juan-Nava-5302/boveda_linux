El comando `sed` (Stream Editor) es una herramienta poderosa para procesar y manipular texto en archivos y flujos de datos. A continuación, se presentan sus características, sintaxis, opciones y algunos ejemplos de uso.

## Características Principales

- **Buscar y reemplazar texto**: Permite buscar patrones y reemplazarlos por otros.
- **Insertar y eliminar líneas**: Puede insertar o eliminar líneas en un archivo sin abrirlo en un editor de texto.
- **Manipulación de texto**: Utiliza expresiones regulares para buscar y manipular patrones complejos.

## Sintaxis General

```bash
sed [opciones] 'script' archivo
```

## Opciones Comunes

- `-e script`: Añade el script a la lista de comandos a ejecutar.
- `-f archivo`: Lee el script desde el archivo especificado.
- `-i[SUF]`: Edita los archivos en el lugar (in-place) y opcionalmente hace una copia de seguridad.
- `-n`: Suprime la salida automática; solo se imprime lo que se especifica explícitamente.
- `-r`: Usa expresiones regulares extendidas.
- `-s`: Trata cada archivo de entrada por separado.

## Ejemplos de Uso

### Buscar y Reemplazar Texto

Reemplaza la primera aparición de "viejo" por "nuevo" en cada línea del archivo:

```bash
sed 's/viejo/nuevo/' archivo.txt
```

Reemplaza todas las apariciones de "viejo" por "nuevo" en cada línea del archivo:

```bash
sed 's/viejo/nuevo/g' archivo.txt
```

### Reemplazar en una Línea Específica

Reemplaza "viejo" por "nuevo" solo en la segunda línea del archivo:

```bash
sed '2s/viejo/nuevo/' archivo.txt
```

### Eliminar Líneas

Elimina la primera línea del archivo:

```bash
sed '1d' archivo.txt
```

Elimina las líneas de la 2 a la 4 del archivo:

```bash
sed '2,4d' archivo.txt
```

### Insertar Texto

Inserta "nuevo texto" antes de la segunda línea del archivo:

```bash
sed '2i\nuevo texto' archivo.txt
```

### Guardar Cambios en el Mismo Archivo

Para aplicar los cambios directamente en el archivo original:

```bash
sed -i 's/viejo/nuevo/g' archivo.txt
```