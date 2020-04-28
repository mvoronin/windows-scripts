# windows-scripts

## Swapping CAPS and left Ctrl

Here is the short explanation of the long string of digits we add to the Scancode Map key in the swap_ctrl_caps.reg file.

00,00,00,00  Header: Version. Set to all zeroes.
00,00,00,00  Header: Flags. Set to all zeroes.
03,00,00,00  3 entries in the map, including null entry.
1d,00,3a,00  Left Ctrl -> CAPS.
3a,00,1d,00  CAPS -> Left Ctrl.
00,00,00,00  Null entry.

Some other keys' codes:

3a 00    CAPS
1d 00    Left Ctrl
1d e0    Right Ctrl
38 00    Left Alt
38 e0    Right Alt
5b e0    Left Windows Key
5c e0    Right Windows Key
5d e0    Windows Menu Key
