<!--
https://pypi.org/project/readme-generator/
https://pypi.org/project/python-readme-generator/
-->

[![](https://img.shields.io/badge/OS-macOS-blue.svg?longCache=True)]()
[![](https://img.shields.io/pypi/v/mac-terminal-interpreter.svg?maxAge=3600)](https://pypi.org/project/mac-terminal-interpreter/)
[![](https://img.shields.io/npm/v/mac-terminal-interpreter.svg?maxAge=3600)](https://www.npmjs.com/package/mac-terminal-interpreter)
[![Travis](https://api.travis-ci.org/looking-for-a-job/mac-terminal-interpreter.svg?branch=master)](https://travis-ci.org/looking-for-a-job/mac-terminal-interpreter/)

#### Installation
```bash
$ [sudo] npm i -g mac-terminal-interpreter
```
```bash
$ [sudo] pip install mac-terminal-interpreter
```

#### Benefits
+   opens in the `Terminal.app` even without `.command` extension
+   stdout, stderr logs
+   makes `.command` file executable
+   window closure options (doesn't close, close if the shell exited cleanly, close always,)
+   displayed non-zero exit status
+   bell notification on error

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

#### Scripts usage
command|`usage`
-|-
`terminal` |`usage: terminal path`

<p align="center">
    <a href="https://pypi.org/project/python-readme-generator/">python-readme-generator</a>
</p>