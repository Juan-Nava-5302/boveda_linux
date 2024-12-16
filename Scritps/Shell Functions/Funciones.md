## ¿Por qué usar funciones?

## ¿Cómo crear funciones? 

#!/bin/bash
function hola() {
 #code goes here.
echo "Hola!"
}

adios() {
 #code goes here.
echo "Adios!"
}

#como llamarla
hola

adios


## ¿Cómo usarlos? 

#!/bin/bash
function hola() {
 #code goes here.
echo "Hola!"
now
}

function now(){
echo "It´s $(date +%r)"
}

hola
      

## Variable scope

## Parámetros de función

### Variables globales

#!/bin/bash
function hola() {
 #code goes here.
echo "Hola $1 !"
}

hola Juancho

Por default las variables son globales.
Las variables deben ser definidas antes de ser usadas.

#!/bin/bash
my_function(){
        GLOBAL_VAR=1
}
/# GLOBAL_VAR not available yet.
echo $GLOBAL_VAR
my_function
/# GLOBAL_VAR is NOW available.
echo $GLOBAL_VAR

Se puede observar que hay 2 llamadas a la variable en consola. El primero se ignora porque aún no se ha llamado a la función que define la variable.

### Variables Locales

Sólo se puede acceder dentro de una función.
Se crea usando la palabra clave "local"
	local LOCAL_VAR = 1
Sólo las funciones usan variables locales

## Estatus de salida y retorno

Cada función tiene un estado de salida. 
De forma explícita: 
	return <RETURN_CODE>
De forma implícita:
	El resultado del último comando ejecutado
Los valores válidos son de 0 a 255, el 0 representa éxito.

