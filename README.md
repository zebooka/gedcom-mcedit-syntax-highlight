# GEDCOM files syntax highlight for mcedit of Midnight Commander

## Installation

1. Copy `$PREFIX/share/mc/syntax/Syntax` to `/home/$USER/.local/share/mc/syntax/Syntax`. `$USER` represents your username.
2. Copy `gedcom.syntax` to `/home/$USER/.local/share/mc/syntax/gedcom.syntax`.
3. Add these two lines at the end of Syntax file, right before unknown files handling (last section):
   ```bash
   file ..\*\\.ged$ GEDCOM
   include /home/$USER/.local/share/mc/syntax/gedcom.syntax
   ```
   Path to `gedcom.syntax` must be absolute.

