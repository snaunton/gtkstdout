# gtkstdout
Gtk application which allows you to run a command and capture and display the output.

usage: gtkstdout [-h] [-0] [-c] [-d DIR] [-t TITLE] COMMAND_LINE ...

Execute a command and display output in a gtk scrolling window

positional arguments:
  COMMAND_LINE          the command line to execute

optional arguments:
  -h, --help            show this help message and exit
  -0, --zero            always return 0
  -c, --close           close immediately after command has finished executing
  -d DIR, --dir DIR     set the working directory
  -t TITLE, --title TITLE
                        set the window title

If the -0/--zero option is not used, a return code of 255 is returned if
cancelled, otherwise the return code of the command executed is returned
<<<<<<< HEAD
=======

>>>>>>> e52703c54866a3fb8249edd676e7d438de278472
