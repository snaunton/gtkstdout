# gtkstdout
Gtk application which allows you to run a command and capture and display the output.

usage: gtkstdout [-h] [-0] [-c] [-d DIR] [-e] [-p] [-x 0-255] [-wi FILE]
                 [-wt TITLE] [-wx PX] [-wy PX]
                 COMMAND_LINE ...

Execute a command and display output in a gtk scrolling window

positional arguments:
  COMMAND_LINE          the command line to execute

optional arguments:
  -h, --help            show this help message and exit
  -0, --zero            always return exit code 0
  -c, --close           close immediately after command has finished executing
  -d DIR, --dir DIR     set the working directory
  -e, --stderr          display stderr also
  -p, --print           echo command output to stdout
  -x 0-255, --exit-code 0-255
                        return this exit code if user cancels
  -wi FILE, --window-icon FILE
                        set window icon
  -wt TITLE, --window-title TITLE
                        set the window title
  -wx PX, --window-width PX
                        set window width in pixels
  -wy PX, --window-height PX
                        set window height in pixels

Returns the exit code of command executed (unless -0/--zero is specified, or
-x/--exit-code is specified and user cancels)
