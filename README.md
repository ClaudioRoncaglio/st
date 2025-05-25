
# st - simple terminal
st is a simple terminal emulator for X which sucks less.

Questa è la mia configurazione personalizzata del terminale

## Patch installate
- gruvbox
- alpha (per la trasparenza)
- scrollback con ring buffer
- scrollback con mouse wheel
- blinking cursor
- font2 - per usare altri font per caratteri non presenti in quello principale
- anysize - per un resizing corretto quando la finestra non è un esatto multiplo dei caratteri


## Requirements
In order to build st you need the Xlib header files.


## Installation
Edit config.mk to match your local setup (st is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install st (if
necessary as root):

```
    make clean install
```

## Running st
If you did not install st with make clean install, you must compile
the st terminfo entry with the following command:

```
    tic -sx st.info
```

See the man page for additional details.

## Credits
Based on Aurélien APTEL <aurelien dot aptel at gmail dot com> bt source code.

