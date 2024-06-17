# Note
I created this mostly for personal use when setting up new machines.

# VSCode settings & hotkeys
The built-in VSCode Zen mode introduced in 2016 is great, but not as customizable as the rest of Code settings.

The core goal of these settings files is to quickly toggle between a "soft" zen mode (I call it "Zen-ish") and full debug mode — the former useful when focusing on writing new functionality (or writing text) and the latter when debugging, enforcing style guides or evaluating code. The quick toggle is helpful when wanting compiler features like codelens or code error highlighting temporarily while writing new functionality.

Obviously, you are free to use these modes however you like.

Depends on the [settings cycler VSCode extension](https://marketplace.visualstudio.com/items?itemName=hoovercj.vscode-settings-cycler) to toggle between zen-ish and debug mode.

This repo also has my extensions manifest, just so I can remember which versions I was using when things were working well!

## Usage
- Install [Settings Cycler extension](https://marketplace.visualstudio.com/items?itemName=hoovercj.vscode-settings-cycler)
- Clone/fork this repo
- [recommended] Hand-merge your VSCode settings into the `settings.json` and `keybindings.json` in the repo folder, if you have any.
- From the repo folder root (macOS, will be different on other OSs/installation configs):
```
rm -rf ~/Library/Application\ Support/Code/User/settings.json
rm -rf ~/Library/Application\ Support/Code/User/keybindings.json
rm -rf ~/.vscode/extensions/extensions.json
ln -s settings.json ~/Library/Application\ Support/Code/User/settings.json
ln -s keybindings.json ~/Library/Application\ Support/Code/User/keybindings.json
ln -s extensions.json ~/.vscode/extensions/extensions.json
```

## Zen-ish mode
No line numbers, bracket guides, indentation guides, VSCode window status bar, command palette, layout buttons, and Codelens annotations (eg: function reference count) on the code.

Compiler errors and warnings are shown in a very dim theme (against a dark mode background) so as to be minimally distracting.

Does *not* hide tabs, sidebar, filepath, or force VSCode into full screen (hiding the taskbar or toolbar) — you can put VSCode into full screen manually each time. For everything but auto-fullscreen toggles you can add parameters to the settings cycler `values`.