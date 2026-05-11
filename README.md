# Visual Studio Code

My VS Code configuration, version-controlled here and symlinked back to where VS Code expects it. Edits made inside VS Code are reflected in this repo directly.

macOS, VS Code.

## Setup on a fresh machine

```sh
# Back up the existing snippets folder if it exists
mv "$HOME/Library/Application Support/Code/User/snippets" \
   "$HOME/Library/Application Support/Code/User/snippets.backup"

# Symlink VS Code's snippets folder to this repo
ln -sf "/path/to/directory/Visual Studio Code" \
   "$HOME/Library/Application Support/Code/User/snippets"
```

VS Code will now read and write snippets directly from this directory. No manual copying needed.

## What's in here

All files are standard VS Code snippet files — one per language.

| File | Language |
|------|----------|
| `css.json` | CSS |
| `html.json` | HTML |
| `javascript.json` | JavaScript |
| `javascriptreact.json` | JSX |
| `markdown.json` | Markdown |
| `shellscript.json` | Shell |
| `typescript.json` | TypeScript |
| `typescriptreact.json` | TSX |
| `vue.json` | Vue |

## Adding snippets

Edit any file directly in VS Code via **Snippets: Configure User Snippets** — changes land in this repo immediately via the symlink. Commit when you're happy with them.
