# Arch package for LTSpice

## Installation

Install with your favorite package helper. (`makepkg -is` or `paru -Ui`)

## Running

Just use the `ltspice` command. (For now `ltspice-help` is broken.)

Please note that running the app requires a `wine` prefix at `~/.local/share/wineprefixes/ltspice`:

    sudo pamac install wine winetricks
    winetricks arch=64 prefix=ltspice

This is a bit tricky to automate in the `PKGBUILD` because it starts an X GUI.

If the font is too small, you can change DPI by running:

    WINEPREFIX=~/.local/share/wineprefixes/ltspice winecfg

