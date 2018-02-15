# autotmux

**autotmux** - Automatically start `tmux` without inception


## Installation

Source `autotmux.sh` at the very **END** of your .\*rc file.

    source /path/to/autotmux.sh [HOSTNAME] [STARTWAIT] [EXITWAIT]

If *HOSTNAME* is not empty, check that $HOSTNAME = *HOSTNAME* before starting (wildcards allowed).  
Waits *STARTWAIT* seconds before starting screen (default 3).   
Waits *EXITWAIT* seconds before exiting the shell after screen terminates (default 2).  

## Usage

When you start your shell, you will be notified that you are about to enter a screen session (^C to cancel).  
When your screen session ends, you will be notified that your shell will exit (^C to cancel).  
You can skip the countdown with any key besides ^C.  

For help using **tmux** see the [tmux manual](http://man.openbsd.org/OpenBSD-current/man1/tmux.1).

## Dependencies

* bash
* screen
