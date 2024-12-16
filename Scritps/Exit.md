## Definir explicitamente el código de retorno

exit 0
exit 1
...

El valor por default es aquel del último comando ejecutado.

ping -c 1 google.com 

ping -c 1 -w 1 amazon.com

ping -c 1 amazon.com.blah

echo "$?"

mkdir -p /tmp/jason/bak && cp -v /etc/hosts /tmp/jason/bak