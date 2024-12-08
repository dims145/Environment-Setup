---
title: VS Code Setup
weight: 1
---

# Download and Install VS Code

# Add Shortcut Default Move Between Tabs

- ctrl+shift+p `Open Keyboard Shortcuts JSON`
- add json

```json
[
    {
        "key": "ctrl+tab",
        "command": "workbench.action.nextEditor"
    },
    {
        "key": "ctrl+shift+tab",
        "command": "workbench.action.previousEditor"
    },
    {
        "key": "ctrl+right",
        "command": "cursorWordEndRight",
        "when": "textInputFocus && !accessibilityModeEnabled"
    },
    {
        "key": "ctrl+left",
        "command": "cursorWordEndLeft",
        "when": "textInputFocus && !accessibilityModeEnabled"
    },
    {
        "key": "alt+right",
        "command": "cursorLineEnd"
    },
    {
        "key": "alt+left",
        "command": "cursorLineStart"
    }
]
```

# Set git bash as Default Terminal

- open settings json -> ctrl+shift+p -> settings json
- appends:

```json
{
    "terminal.integrated.profiles.windows": {
        "Git Bash": {
            "path": "C:\\Program Files\\Git\\bin\\bash.exe"
        },
    },
    "terminal.integrated.defaultProfile.windows": "Git Bash"
}
```
