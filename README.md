USAGE: make-bfil-parfile.py <input box file> <image file> <options>
additional options:
 -f	to flip over y-axis
 -r	to round to nearest whole number
 
run with --help flag to see this message

use e2boxer.py to pick the splines along each fibril for straightening.  
Click off the micrograph on the left side to start a new fibril.
(don't do this after the last fibril though)

once par file is written run bfil to get the straightened fibrils

bfil -extract <box width> -split -base <name> -extension mrc -path <where to write images> <par file> 
