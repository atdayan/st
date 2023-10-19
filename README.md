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

Patches
---
The following patches were applied:
* [alpha](https://st.suckless.org/patches/alpha/st-alpha-osc11-20220222-0.8.5.diff)
* [changealpha](https://st.suckless.org/patches/changealpha/st-changealpha-20230519-b44f2ad.diff)
* [font2](https://st.suckless.org/patches/font2/st-font2-0.8.5.diff)
* [hidecursor](https://st.suckless.org/patches/hidecursor/st-hidecursor-0.8.3.diff)
