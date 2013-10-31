Turn off system beep
====================

In bash
-------

    echo 'set bell-style none' >> $HOME/.inputrc

In the console
--------------

    setterm -blength 0

In X11
------

    xset b off

http://www.debian-administration.org/articles/110
