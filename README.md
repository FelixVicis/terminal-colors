# Bash Terminal Colors
#### A python flavored wrapper for coloring terminal output

This service offers ANSI escaped color sequences.
A few colors are offered by name such as:
```
HEADER    light-magenta
OKBLUE    light-blue'
OKGREEN   light-green
WARNING   light-yellow
FAIL      light-red
END       cancels all styling
BOLD      bold
UNDERLINE underline
HIDE      hidden
```

Outside of those, you can use the class `TerminalColors` to
find statically defined colors and styles.


## Example of simple usage
```py
import colors

colors.OKBLUE
# '\x1b[94m'

colors.END
# '\x1b[0m'

print colors.OKBLUE, "This is blue", colors.END
# This is blue
```
