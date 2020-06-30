<!--
https://readme42.com
-->



[![](https://img.shields.io/badge/OS-Unix-blue.svg?longCache=True)]()
[![](https://img.shields.io/pypi/v/mac-terminal-interpreter.svg?maxAge=3600)](https://pypi.org/project/mac-terminal-interpreter/)
[![](https://img.shields.io/npm/v/mac-terminal-interpreter.svg?maxAge=3600)](https://www.npmjs.com/package/mac-terminal-interpreter)[![](https://img.shields.io/badge/License-Unlicense-blue.svg?longCache=True)](https://unlicense.org/)
[![](https://github.com/andrewp-as-is/mac-terminal-interpreter/workflows/tests42/badge.svg)](https://github.com/andrewp-as-is/mac-terminal-interpreter/actions)

### Installation
```bash
$ [sudo] pip install mac-terminal-interpreter
```

```bash
$ [sudo] npm i -g mac-terminal-interpreter
```

#### How it works
`script.ext`
```bash
#!/usr/bin/env terminal
...
```

stdout, stderr logs:
```
~/Library/Logs/<slug>/<date>/out.log
~/Library/Logs/<slug>/<date>/err.log
```

#### Config
`~/.bashrc`:
```bash
export MAC_TERMINAL_CLOSE=0 # doesn't close (default)
export MAC_TERMINAL_CLOSE=1 # close if the shell exited cleanly
export MAC_TERMINAL_CLOSE=2 # close always
```

Terminal error sound:
```bash
$ defaults write .GlobalPreferences com.apple.sound.beep.sound /System/Library/Sounds/Basso.aiff
```

<p align="center">
    <a href="https://readme42.com/">readme42.com</a>
</p>