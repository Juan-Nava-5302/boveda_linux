Sintaxis: [condition-to-test-for] 

Ejemplo: [-e /etc/passwd]

File operators (tests)

|                  |                                        |
| ---------------- | -------------------------------------- |
| -d               | True if file is a directory            |
| -e               | T if file exists                       |
| -f               | T if file exists and is a regular file |
| -r               | T if file is readable by you           |
| -s               | T if file exists and is not empty      |
| -w               | T if F is writable by you              |
| -x               | T if f is executable by you            |
| -z               | T I String is empty                    |
| -n               | T I String is not empty                |
| STRING1=STRING2  | T if strings are equal                 |
| STRING1!=STRING2 | T if strings are different             |

Arithmetic op (tests)

|   |   |
|---|---|
|Arg1 -eq arg2|T If both are equal|
|Arg1 -ne arg2|T if both equal|
|Arg1 –(L)lt arg2|T if arg1<arg2|
|Arg1 –(L) le arg2|T if arg1 <= arg2|
|Arg1 -gt arg2|T if arg1 >arg2|
|Arg1 -ge arg2|T I arg1 >= arg2|

help