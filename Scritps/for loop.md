#!/bin/bash
for COLOR in red green blue
do
        echo "COLOR: $COLOR"
done

------------
may use a list for the values

#!/bin/bash
COLORS="red green blue"

for COLOR in $COLORS
do
        echo "COLOR: $COLOR"
done

------------------
