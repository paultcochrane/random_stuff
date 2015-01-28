# Set up the console keymap

## Initial configuration

    $ sudo dpkg-reconfigure keyboard-configuration
    -> Generic 105-key (Intl) PC
    -> US international AltGr dead keys
    -> Key to function as AltGr: Right Alt (AltGr)
    -> Compose key: No compose key
    -> Use Control+Alt+Backaspace to terminate X server
    # load the settings into the running console
    $ sudo /etc/init.d/keyboard-setup

## Set up mappings to special characters

  * `AltGr+a => ä`

    $ echo 'keycode 30 = +a +A +adiaeresis +Adiaeresis' | sudo loadkeys

  * `AltGr+o => ö`

    $ echo 'keycode 24 = +o +O +odiaeresis +Odiaeresis' | sudo loadkeys

  * `AltGr+u => ü`

    $ echo 'keycode 22 = +u +U +udiaeresis +Udiaeresis' | sudo loadkeys

  * `AltGr+s => ß`

    $ echo 'keycode 31 = +s +S +ssharp' | sudo loadkeys
