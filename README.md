# opener
Shell based file opener using mimetypes as well as file extension. This does not depend on desktop files. 

How to use:

open $file

    opener $file

search file using fzf and open

    opener "$(find . -type f | fzf --border --reverse --height 10 --prompt "Open File : ")"
This can be a function in .bashrc
        of() {
        opener "$(find . -type f | fzf --border --reverse --height 10 --prompt "Open File : ")"
        }


How to configure:
find the mimetype of file using

    file -bi $file

and add the mimetype with commands to open it in opener.

Here is video to show my workflow using run, opener and w3m-dmenu scripts.
https://youtu.be/e5Lutp0dWTk
