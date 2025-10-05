PyCalc-NG
=========

**Infinite-precision desktop calculator app in ~50 lines of Python.**
No other dependencies—all the features. 🙌

[![Build status](https://img.shields.io/github/actions/workflow/status/kernc/pycalc-ng/ci.yml?branch=master&style=for-the-badge)](https://github.com/kernc/pycalc-ng/actions)
[![Language: shell / Bash](https://img.shields.io/badge/lang-Shell-peachpuff?style=for-the-badge)](https://github.com/kernc/pycalc-ng)
[![Language: Python](https://img.shields.io/badge/lang-Python-blue?style=for-the-badge)](https://github.com/kernc/pycalc-ng)
[![Source lines of code](https://img.shields.io/endpoint?url=https%3A%2F%2Fghloc.vercel.app%2Fapi%2Fkernc%2Fpycalc-ng%2Fbadge?filter=pycalc%26format=human&style=for-the-badge&label=SLOC&color=skyblue)](https://ghloc.vercel.app/kernc/pycalc-ng)
[![Script size](https://img.shields.io/github/size/kernc/pycalc-ng/pycalc?style=for-the-badge&color=skyblue)](https://github.com/kernc/pycalc-ng)
[![Issues](https://img.shields.io/github/issues/kernc/pycalc-ng?style=for-the-badge)](https://github.com/kernc/pycalc-ng/issues)

Made as a dead-simple wrapper around Python that preimports
stuff from its **_math_ and _statistics_ modules** (including _numpy_, if available)
before dropping into the familiar REPL.

This replaces the functionality of several modern command-driven scientific calculators,
as available e.g. in Debian,
at less than half the source code lines spent! YMMV


Installation
------------
Download the script and put it somewhere on `$PATH`:
```sh
curl -vL 'https://bit.ly/pycalc-ng' | sudo tee /usr/local/bin/pycalc
sudo chmod +x /usr/local/bin/pycalc  # Mark it executable
```

Make sure Python 3 is available:
```sh
sudo apt install python3
```

A terminal emulator (`xterm` from _x11-utils_ (recommended), `gnome-terminal` or `konsole`)
serves as a simple GUI:
```sh
sudo apt install x11-utils
```
If you use a tiling window manager,
like _i3_, _awesome_, _xmonad_ or _dwm_,
additional utilities `xprop` and `xdotool` are required
to make the app window dialog-like (floating):
```sh
sudo apt install x11-utils xdotool
```

If you prefer a more full-featured Python REPL, such as _ptpython_ or _ipython3_
with syntax highlighting and <kbd>Tab</kbd>-based autocompletion,
those are automatically used if found!
```sh
sudo apt install ptpython  # or ipython3
```

Usage
-----
Simple invocation should spawn a new app window:
```sh
$ pycalc
```
... in which you can type your fancy equations:
```python-repl
>>> 1+1
2
```
Supports variable assignment just like Python does. Etc. 😋
