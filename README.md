# gtkstdout
Gtk application which allows you to run a command and capture and display the output.

Execute a command and display output in a gtk scrolling window

positional arguments:
  COMMAND_LINE          the command line to execute

optional arguments:
  -h, --help            show this help message and exit
  -0, --zero            always return 0
  -c, --close           close immediately after command has finished executing
  -d DIR, --dir DIR     set the working directory
  -e, --stderr          display stderr also
  -i FILE, --icon FILE  set window icon
  -x 0-255, --exit-code 0-255
                        exit code if user cancels
  -t TITLE, --title TITLE
                        set the window title

If the -x/--exit-code and -0/--zero option are not used, or -x/-exit-code is
invalid, an exit code of 255 is returned if the users cancels, otherwise the
exit code of the command executed is returned
