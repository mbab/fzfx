# Development
## Todo
- Write unit testing
- Write CI script to update AUR version
- Write issue templates for bugs and features 

## Features
### Switch modes in-program
I don't think added functionality exceeds extra complexity but apparently 'change-prompt' action can be used for that.

Related: https://github.com/junegunn/fzf/issues/2423 

## Bugs
Full mode is hanging when opening file. What is happening is that queries aren't getting aborted so Fzf hangs in the background waiting queries to finish. Bug is difficult to observe and apparently fixed.

If it is observed again I can try to:

- Report a bug
- Use & to parallelize opening file
- Use killall to terminate query
