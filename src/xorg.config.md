# Xorg configuration

## Snippets

### Keyboard

```
Section "InputClass"
    Identifier "Keyboard"
    MatchIsKeyboard "on"
    Option "XkbLayout" "us,ru"
    Option "XkbModel" "pc104"
    Option "XkbOptions" "grp:caps_toggle"
EndSection
```

### Logi TrackMan Marble

Scroll with trackball, small left button pressed:

```
Section "InputClass"
    Identifier   "Marble Mouse"
    MatchProduct "Logitech USB Trackball"
    Driver       "libinput"
    Option       "ScrollMethod"    "button"
    Option       "ScrollButton"    "8"
    Option       "MiddleEmulation" "true"
EndSection
```

[Arch wiki page about trackman](https://wiki.archlinux.org/index.php/Logitech_Marble_Mouse)
