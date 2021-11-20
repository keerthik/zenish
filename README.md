# VSCode settings & hotkeys

The built-in VSCode Zen mode introduced in 2016 is great, but not as customizable as the rest of Code settings.

The core goal of these settings files is to quickly toggle between a "soft" zen mode (I call it "Zen-ish") and full debug mode — the former useful when focusing on writing new functionality (or writing prose) and the latter when debugging, enforcing style guides or evaluating code. The quick toggle is helpful when wanting compiler features like codelens or code error highlighting temporarily while writing new functionality.

Obviously, you are free to use these modes however you like.

Depends on the [settings cycler VSCode plugin](https://marketplace.visualstudio.com/items?itemName=hoovercj.vscode-settings-cycler) to toggle between zen-ish and debug mode.

## Zen-ish mode
No line numbers, bracket guides, indentation guides, VSCode status bar, VSCode "code-lens" annotations on the code.

Compiler errors and warnings are shown in a very dim theme (against a dark mode background) so as to be minimally distracting.

Does *not* hide tabs, sidebar, filepath, or force VSCode into full screen (hiding the taskbar or toolbar) — you can put VSCode into full screen manually each time. For everything but auto-fullscreen toggles you can add parameters to the settings cycler `values`.