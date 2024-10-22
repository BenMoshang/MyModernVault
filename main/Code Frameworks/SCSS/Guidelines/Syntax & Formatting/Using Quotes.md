- *==CSS does not require strings to be quoted==,* not even those containing spaces.
it doesn’t matter whether you wrap them in quotes for the CSS parser.

- That being said, languages that do not require strings to be quoted are definitely a minority and so....

## Why:
- **strings should always be wrapped with single quotes** (`'`) in Sass 

- Besides consistency with other languages, including CSS’ cousin JavaScript, there are several reasons for this choice:

<font color="#eeece1">- color names are treated as colors when unquoted, which can lead to serious issues</font>
<font color="#eeece1">	- most syntax highlighters will choke on unquoted strings;</font>
<font color="#eeece1">	- it helps general readability;</font>
<font color="#eeece1">	- there is no valid reason not to quote strings.</font>
	- ![[Pasted image 20241022085912.png]]