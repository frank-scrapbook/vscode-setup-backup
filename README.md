# vscode-setup-backup

## Backups
- Extensions
- Settings Profile
- settings.json
- keybindings.json


## Manual
### Backup Extensions
Get Extension IDs into a text file.

Example Usage: 
```
code --list-extensions >> extensions-list-20231107.txt
```

Example Usage (with reference to specific vscode settings profile):
```
code --profile "General Work Laptop" --list-extensions >> extensions-list-20231107.txt
```

### Backup Settings Profile (File Extension: .code-profile)
macOS (specific vscode settings profile, either "Default" or custom "General Work Laptop"):
```
Code (Application Name, next to Apple Symbol) --> Settings... --> Profiles (General Work Laptop) --> Export Profile... --> Export (button) --> Export (button) --> Export (as Local file)
```

NOTE: my "Default" profile is not really default. Still contains "Dev Containers" and "Docker" vscode extensions.

### Backup settings.json
macOS:
```
Cmd + ,
```

Top Right Corner, File Logo with Arrow for "Open Settings (JSON)"

File Path (for default installs): 
```
~/Library/Application Support/Code/User/settings.json
```

Example Usage (macOS Terminal - copy settings.json to current directory):
```
cp ~/Library/"Application Support"/Code/User/settings.json .
```

### Backup keybindings.json
macOS:
```
Cmd+K Cmd+S
```

Top Right Corner, File Logo with Arrow for "Open Keyboard Shortcuts (JSON)"

File Path (for default installs):
```
~/Library/Application Support/Code/User/keybindings.json
```

Example Usage (macOS Terminal - copy keybindings.json to current directory):
```
cp ~/Library/"Application Support"/Code/User/keybindings.json .
```

## Automated
### Command Palette
macOS: 
```
Cmd + Shift + P
```

### Command Palette: Settings Sync
macOS:
```
> Settings Sync: Configure
> Settings Sync: Show Synced Data
```

Can Sync to GitHub or Microsoft

## References
- https://code.visualstudio.com/docs/editor/profiles
- https://code.visualstudio.com/docs/editor/settings-sync
  - https://code.visualstudio.com/docs/editor/settings-sync#_synced-machines