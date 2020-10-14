st - simple terminal
--------------------
st is a simple terminal emulator for X which sucks less.


Requirements
------------
In order to build st you need the Xlib header files.


Installation
------------
Edit config.mk to match your local setup (st is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install st (if
necessary as root):

    make clean install


Patches applied
---------------
- [st-alpha-0.8.2.diff](https://st.suckless.org/patches/alpha/)
- [st-anysize-0.8.1.diff](https://st.suckless.org/patches/anysize/)
- [st-blinking_cursor-20200531-a2a7044.diff](https://st.suckless.org/patches/blinking_cursor/)
- [st-dracula-0.8.2.diff](https://st.suckless.org/patches/dracula/)
- [st-scrollback-20200419-72e3f6c.diff](https://st.suckless.org/patches/scrollback/)


Running st
----------
If you did not install st with make clean install, you must compile
the st terminfo entry with the following command:

    tic -sx st.info

See the man page for additional details.

Credits
-------
Based on Aurélien APTEL <aurelien dot aptel at gmail dot com> bt source code.

