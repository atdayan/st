st - simple terminal
---
This is a fork of the st project, which is maintained by the
[suckless](https://st.suckless.org) team.
The goal of this project is to be a simple and lightweight terminal
emulator.

Requirements
---
In order to build st you need the Xlib header files.

Installation
---
The program will be installed under `$HOME/.local` by default. You can
change the installation path by editing the `config.mk` file. Make sure
that `$HOME/.local/bin` is in your `PATH` variable.

```
make clean install
```

If you want no terminfo folder in your home directory, export the
`TERMINFO=$HOME/.local/share/terminfo` variable in your shell
configuration file.

Customization
---
The default configuration is `config.def.h`. To make changes, edit the
generated `config.h` file. After the customizations are done, rebuild the
project as instructed in the previous section.
