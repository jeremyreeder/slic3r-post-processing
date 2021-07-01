# slic3r-post-processing
Post-processing scripts for Slic3r/Prusaslicer

## Installation

These files can be kept anywhere accessible, but personally I put them in
~/.config/PrusaSlicer/post/.

## Configuration

In your slicer, go to: Print Settings > Output options. Add the full path of
one or more of these scripts to the 'Post-processing scripts' field.

Go to: Printer Settings > Custom G-code. In the 'Start G-code' field, set
parameters for each script as indicated below.

## temperature_offset

This script corrects for thermistor discrepancies between printers, based on
specified correction offsets. Configure as follows, in the 'Start G-code'
field, at some point prior to the first temperature-relate commands.

;TEMPERATURE_OFFSET:-6
;BED_TEMPERATURE_OFFSET:3
