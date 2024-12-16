## ¿Qué son?

Un caracter o string usado para hacer pattern matching.

Globbing expands the wildcard pattern into a list of files and/or directories. (paths)

Wildcards can be used with most commands.

	ls 
	rm 
	cp

- * matches zero or more characters
	- *.txt
	- a*
	- a*.txt
- ? matches exactly one character
	- ?.txt
	- a?
	- a?.txt

- [] A character class.
	- Matches any of the characters included between the brackets. Matches exactly one character.
	- [aeiou]
	- ca[nt]*
		- can
		- cat
		- candy
		- catch
- [!] Matches any of the characters NOT included between the brackets. Matches exactly one character.
	- [!aeiou]*
	- baseball
	- cricket
- [a-g]* Ranges. Use two caracters separated by a hyphen to create a range in a character class. Matches all files that start with a,b,c,d,e,f,or g.
- [3-6]* Matches all files that start with 3,4,5, or 6.

### Named character classes

- [[:alpha:]]: Matches any alphabetic character, both uppercase and lowercase (A-Z, a-z). It is equivalent to `[A-Za-z]`.
    
- [[:alnum:]]: Matches any alphanumeric character, which includes alphabetic characters (both uppercase and lowercase) and digits (0-9). It is equivalent to `[A-Za-z0-9]`.
    
- [[:digit:]]: Matches any digit (0-9). It is equivalent to `[0-9]`.
    
- [[:lower:]]: Matches any lowercase alphabetic character (a-z). It is equivalent to `[a-z]`.
    
- [[:space:]]: Matches any whitespace character, including spaces, tabs, and newlines. It is equivalent to `[\t\n\r\f\v]`.
    
- [[:upper:]]: Matches any uppercase alphabetic character (A-Z). It is equivalent to `[A-Z]`.

### Matching Wildcard patterns
- / escape character. Use if you want to match a wildcard character.
	- Match all files that end with a question mark:
		- 
## ¿Cuándo y dónde usarlos?
*\?
	done?
## Tipos

## Cómo usarlos con varios comandos


[jason@linuxsvr bin]$ 