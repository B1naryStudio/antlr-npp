Notepad++ improvements for ANLTR grammar syntax highlighting and debugging

1. Add syntax highlighting
Use menu Language->Define your language...->Import... and choose antlr4_highlight.xml

2. Add debug scripts
Install plugin "NppExec" using standard "Plugin Manager".
When it has finished open NppExec menu and choose "Execute...".  Copy-paste content from one of *.nppexec file, change path to your ANTLR jar, and save it with some name.
Now if you open NppExec "Advanced Options..." you can choose your script at the left bottom and add it to Notepad++ "Macro" menu.
Once you've added it there you can bind hot-key to it using Notepad++ standard way: Settings->Shortcut mapper...->Plugin commands.

Scripts use currently opened file as grammar file and selected text as root rule for visualization. 
So to use it open grammar file, make name of tested rule selected then run script and input some test data.

run_user_input.nppexec - asks one line to use as parser input

run_file_input.nppexec - asks file name to parse file