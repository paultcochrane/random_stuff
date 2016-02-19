# awesome Window Manager

Close currently selected window
    Mod4-Shift-c

## Running Java programs

    $ sudo aptitude install wmname  # in case it isn't installed
    $ wmname LG3D
    $ <start-java-program>

Much more information available at the Awesome website:

https://awesome.naquadah.org/wiki/Problems_with_Java#OpenJDK

## Allow awesome to show up in the GDM greeter

On a Debian system, awesome won't show up in the GDM greeter after it has
been installed.  This can be annoying on multi-user systems where one person
wants to use awesome and another wishes to use another window manager.  It
turns out that the default setting is *not* to show awesome in the list of
available window managers in the greeter.  The solution is to set the
`NoDisplay=true` line in `/usr/share/xsessions/awesome.desktop` to `false.
I.e. this:

    [Desktop Entry]
    Encoding=UTF-8
    Name=awesome
    Comment=Highly configurable framework window manager
    NoDisplay=true
    TryExec=awesome
    Exec=awesome
    Type=Application

becomes this:

    [Desktop Entry]
    Encoding=UTF-8
    Name=awesome
    Comment=Highly configurable framework window manager
    NoDisplay=false
    TryExec=awesome
    Exec=awesome
    Type=Application
