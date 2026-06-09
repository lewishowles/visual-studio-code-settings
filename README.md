# Visual Studio Code

My VS Code configuration, version-controlled here and symlinked back to where VS Code expects it. Edits made inside VS Code are reflected in this repo directly.

## Setup on a fresh machine

```sh
# Back up the existing snippets folder if it exists
mv "$HOME/Library/Application Support/Code/User/snippets" "$HOME/Library/Application Support/Code/User/snippets.backup"
mv "$HOME/Library/Application Support/Code/User/settings.json" "$HOME/Library/Application Support/Code/User/settings.json.backup"

# Symlink VS Code's snippets folder to this repo, run from the repo itself.
ln -sfn "$(pwd)/snippets" "$HOME/Library/Application Support/Code/User/snippets"

# Symlink VS Code's settings to this repo
ln -sf "$(pwd)/settings.json" "$HOME/Library/Application Support/Code/User/settings.json"
```

VS Code will now read and write snippets and settings directly from this directory.
