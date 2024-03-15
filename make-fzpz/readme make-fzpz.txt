Creates a *.fzpz file for a single Fritzing part. Requires application
7-Zip (7z.exe) to be in the path.

  make-fzpz [/?|-h|--help] <partname>

<partname>     Name of the Fritzing part. The name must not include
               spaces.
/?|-h|--help   Displays this message.

The *.fzp and *.svg files for the part are assumed to exist in folders
\part, \svg\icon, \svg\breadboard, \svg\schematic and \svg\pcb, with names
<partname>.fzp
<partname>_<view>.svg

Where <view> is one of icon, breadboard, schematic or pcb.

