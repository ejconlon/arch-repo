# LTSpice

Forked from the [AUR](https://aur.archlinux.org/packages/ltspice).

Use the `ltspice` command to start the program. (For now `ltspice-help` is broken.)

Please note that running the app first requires a `wine` prefix at `~/.local/share/wineprefixes/ltspice`:

    sudo pamac install wine winetricks
    winetricks arch=64 prefix=ltspice

This is a bit tricky to automate in the `PKGBUILD` because it starts an X GUI.

If the font is too small, you can change DPI by running:

    WINEPREFIX=~/.local/share/wineprefixes/ltspice winecfg

