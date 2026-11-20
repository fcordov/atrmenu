# BF loader

A single-file, 100% offline web tool that builds Atari 8-bit `.ATR` disk images with a bootable, selectable menu. Open `atrmenu.html` in any modern browser. There is nothing to install and nothing is uploaded.

## What it does

**Step 1 – Files → ATR**
- Drop `.XEX` / `.BIN` / `.COM` files to build a disk from scratch, or drop an existing `.ATR` to jump straight to the menu step.
- Blank disk formats: SD 90 KB, MD 130 KB (enhanced), DD 180 KB, QD 360 KB, DS/QD 720 KB, or **custom geometry** (sector count, boot sectors, and 128/256/512-byte sectors).
- Live capacity bar. Files on a loaded ATR can be downloaded or deleted.
- **Export ATR without menu**, optionally with a bootable DOS: Atari DOS 2.5, DOS II+ or MyDOS 4.5.

**Step 2 – Disk menu**
- Builds a disk that boots straight into your menu, with no DOS required.
- Press `1`–`9` or `A`–`Z` to load a program. Up to 128 entries.
- Layout adapts to the entry count: one column, then two columns, then multiple pages. Flip pages with `, .` / `< >` / `+ -` / SPACE / arrow keys.
- Editable title and labels. Order entries manually or alphabetically (A→Z / Z→A).
- Background color, text contrast and invert-colors controls, with a live 40×24 Atari-style preview.
- The menu footer shows used/total disk capacity and the "BF loader" tag.

**Interface**
- English (default) and Spanish, switchable from the top-right button.

## Notes
- The menu replaces the DOS boot sector. Programs are loaded with a built-in Atari binary-load routine, so they should be standard XEX/binary-load files.
- On the Atari's text screen, the text hue always follows the background. Only its brightness can differ.
- The preview colors approximate an NTSC Atari and may differ slightly from your emulator or screen.
- 512-byte-sector disks use a simplified layout that the menu loader reads but DOS does not.
