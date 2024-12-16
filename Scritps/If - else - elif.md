
## If

Recordar que debe de haber un espacio en los if entre los corchetes y el comando de la condición.

#!/bin/bash
MY_SHELL="bash"

if [ "$MY_SHELL" = "bash" ]
then
        echo "You seem to like the bash shell."
fi


## If / else

#!/bin/bash
MY_SHELL="lol en plan omg"

if [ "$MY_SHELL" = "bash" ]
then
        echo "You seem to like the bash shell."
else
        echo "You don´t seem to like the bash shell."
fi

# elif

X#!/bin/bash
MY_SHELL="lol en plan omg"

if [ "$MY_SHELL" = "bash" ]
then
        echo "You seem to like the bash shell."
elif [ "$MY_SHELL" = "csh" ]
then
        echo "You seem to like the csh shell"
else
        echo "You don´t seem to like the bash or csh shell."
fi
