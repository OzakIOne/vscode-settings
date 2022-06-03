# vscode-settings

## Requirements

settings.json (ctrl shift p > settings json)
```json
  "syncSettings.resources": [
    "extensions",
    "keybindings",
    "settings",
    "snippets",
    "uiState"
  ],
  // "syncSettings.additionalFiles": ["~globalStorage", "~editorStorage"],
```

settings.yml (ctrl shift p > sync settings open repo)
```yml
# # current machine's name, optional; it can be used to filter settings or in the commit message
hostname: 'ozaki-windows-desktop'
# # more details at https://github.com/zokugun/vscode-sync-settings/blob/master/docs/hostname.md
profile: main
# sync on remote git
repository:
  type: git
  # url of the remote git repository to sync with, required
  url: https://github.com/OzakIOne/vscode-settings.git
  # url: git@github.com:OzakIOne/vscode-settings.git
  # branch to sync on, optional (set to `master` by default)
  branch: master
  # how to personalize the commit messages at https://github.com/zokugun/vscode-sync-settings/blob/master/docs/commit-messages.md
```
