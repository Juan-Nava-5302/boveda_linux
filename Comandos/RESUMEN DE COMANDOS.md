Lista de 50 comandos de Linux, lo que hacen y un ejemplo de uso para cada uno:

1. **`ls`**: Lista archivos y directorios.
    
    ```bash
    ls -l
    ```
    
2. **`cd`**: Cambia el directorio actual.
    
    ```bash
    cd /home/usuario
    ```
    
3. **`pwd`**: Muestra el directorio de trabajo actual.
    
    ```bash
    pwd
    ```
    
4. **`cp`**: Copia archivos o directorios.
    
    ```bash
    cp archivo.txt /ruta/destino/
    ```
    
5. **`mv`**: Mueve o renombra archivos o directorios.
    
    ```bash
    mv archivo.txt nuevo_nombre.txt
    ```
    
6. **`rm`**: Elimina archivos o directorios.
    
    ```bash
    rm archivo.txt
    ```
    
7. **`mkdir`**: Crea un nuevo directorio.
    
    ```bash
    mkdir nuevo_directorio
    ```
    
8. **`rmdir`**: Elimina directorios vacíos.
    
    ```bash
    rmdir directorio_vacio
    ```
    
9. **`touch`**: Crea un archivo vacío o actualiza la fecha de modificación.
    
    ```bash
    touch nuevo_archivo.txt
    ```
    
10. **`cat`**: Muestra el contenido de un archivo.
    
    ```bash
    cat archivo.txt
    ```
    
11. **`more`**: Muestra el contenido de un archivo página por página.
    
    ```bash
    more archivo.txt
    ```
    
12. **`less`**: Similar a `more`, pero con más funcionalidades.
    
    ```bash
    less archivo.txt
    ```
    
13. **`head`**: Muestra las primeras líneas de un archivo.
    
    ```bash
    head archivo.txt
    ```
    
14. **`tail`**: Muestra las últimas líneas de un archivo.
    
    ```bash
    tail archivo.txt
    ```
    
15. **`echo`**: Muestra un mensaje en la pantalla.
    
    ```bash
    echo "Hola, mundo"
    ```
    
16. **`grep`**: Busca texto dentro de archivos.
    
    ```bash
    grep "texto" archivo.txt
    ```
    
17. **`find`**: Busca archivos y directorios.
    
    ```bash
    find /ruta -name "archivo.txt"
    ```
    
18. **`locate`**: Encuentra archivos rápidamente usando una base de datos.
    
    ```bash
    locate archivo.txt
    ```
    
19. **`du`**: Muestra el uso de espacio en disco de archivos y directorios.
    
    ```bash
    du -sh /ruta/del/directorio
    ```
    
20. **`df`**: Muestra el uso de espacio en disco de los sistemas de archivos.
    
    ```bash
    df -h
    ```
    
21. **`chmod`**: Cambia los permisos de archivos o directorios.
    
    ```bash
    chmod 755 archivo.sh
    ```
    
22. **`chown`**: Cambia el propietario de archivos o directorios.
    
    ```bash
    chown usuario:grupo archivo.txt
    ```
    
23. **`ps`**: Muestra los procesos en ejecución.
    
    ```bash
    ps aux
    ```
    
24. **`top`**: Muestra los procesos en ejecución en tiempo real.
    
    ```bash
    top
    ```
    
25. **`kill`**: Termina un proceso.
    
    ```bash
    kill 1234
    ```
    
26. **`ping`**: Comprueba la conectividad de red.
    
    ```bash
    ping google.com
    ```
    
27. **`ifconfig`**: Configura interfaces de red.
    
    ```bash
    ifconfig
    ```
    
28. **`ip`**: Muestra y manipula la configuración de red.
    
    ```bash
    ip addr show
    ```
    
29. **`netstat`**: Muestra estadísticas de red.
    
    ```bash
    netstat -tuln
    ```
    
30. **`route`**: Muestra y manipula la tabla de enrutamiento.
    
    ```bash
    route -n
    ```
    
31. **`wget`**: Descarga archivos de la web.
    
    ```bash
    wget https://ejemplo.com/archivo.zip
    ```
    
32. **`curl`**: Transfiere datos desde o hacia un servidor.
    
    ```bash
    curl https://ejemplo.com
    ```
    
33. **`scp`**: Copia archivos entre hosts de manera segura.
    
    ```bash
    scp archivo.txt usuario@host:/ruta/destino
    ```
    
34. **`ssh`**: Conecta a un host remoto de manera segura.
    
    ```bash
    ssh usuario@host
    ```
    
35. **`nano`**: Editor de texto simple.
    
    ```bash
    nano archivo.txt
    ```
    
36. **`vim`**: Editor de texto avanzado.
    
    ```bash
    vim archivo.txt
    ```
    
37. **`tar`**: Archiva y descomprime archivos.
    
    ```bash
    tar -czvf archivo.tar.gz /ruta/del/directorio
    ```
    
38. **`gzip`**: Comprime archivos.
    
    ```bash
    gzip archivo.txt
    ```
    
39. **`gunzip`**: Descomprime archivos.
    
    ```bash
    gunzip archivo.txt.gz
    ```
    
40. **`zip`**: Comprime archivos en formato ZIP.
    
    ```bash
    zip archivo.zip archivo.txt
    ```
    
41. **`unzip`**: Descomprime archivos ZIP.
    
    ```bash
    unzip archivo.zip
    ```
    
42. **`history`**: Muestra el historial de comandos.
    
    ```bash
    history
    ```
    
43. **`alias`**: Crea un alias para un comando.
    
    ```bash
    alias ll='ls -la'
    ```
    
44. **`unalias`**: Elimina un alias.
    
    ```bash
    unalias ll
    ```
    
45. **`free`**: Muestra el uso de memoria del sistema.
    
    ```bash
    free -h
    ```
    
46. **`uname`**: Muestra información del sistema.
    
    ```bash
    uname -a
    ```
    
47. **`who`**: Muestra quién está conectado al sistema.
    
    ```bash
    who
    ```
    
48. **`su`**: Cambia a otro usuario.
    
    ```bash
    su - usuario
    ```
    
49. **`sudo`**: Ejecuta comandos con privilegios de superusuario.
    
    ```bash
    sudo comando
    ```
    
50. **`crontab`**: Programa tareas para que se ejecuten periódicamente.
    
    ```bash
    crontab -e
    ```
    

Espero que esta lista te sea útil para tus tareas en Linux. ¿Hay algún comando en particular sobre el que te gustaría más detalles?