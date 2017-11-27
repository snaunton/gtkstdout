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
  -0, --zero            always return an exit status of 0
  -c, --close           close immediately after command has finished executing
  -d DIR, --dir DIR     set the working directory
  -e, --stderr          display stderr also
  -p, --print           echo command output to stdout
  -x 0-255, --exit-status 0-255
                        return this exit status if user cancels
  -wi FILE, --window-icon FILE
                        set window icon
  -wt TITLE, --window-title TITLE
                        set the window title
  -wx PX, --window-width PX
                        set window width in pixels
  -wy PX, --window-height PX
                        set window height in pixels

By default an exit status of 255 is returned if the user cancels, otherwise
the exit status of the command executed is returned. This can be be changed
using --exit-status or --zero. If an invalid value is specified for --exit-
status a value of 255 is used insead. If both --exit-status and --zero are
specified, --exit-status is ignored and 0 will be returned.
