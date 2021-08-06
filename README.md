# opener
Shell based file opener using mimetypes as well as file extension. This does not depend on desktop files. 

How to use:

open $file
[code]opener $file[/code]
search file using fzf and open
[code]opener "$(find . -type f | fzf --border --reverse --height 10 --prompt "Open File : ")"[/code]

How to configure:
find the mimetype of file using 
[code]file -bi $file[/code]
and add the mimetype with commands to open it in opener.
