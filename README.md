# PROJECT: musexmlexport
A utility to extract an ECG rhythm strip from a MUSE(R) XML file. It converts MUSE XML files to CSV files, suitable for import into Excel and MATLAB.

This program is is written for use with **Python 2**.

## Copyright Information
Copyright 2009 GE Healthcare

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program (it is embedded in the text of this script).
If not, see <http://www.gnu.org/licenses/>.

You may contact the author by e-mail (anthony.ricke@med.ge.com). For updates to this software, please visit the
Source Forge project site (http://sourceforge.net/projects/musexmlexport/)

- MUSE is a registered trademark of GE Healthcare, Inc.

## History

- Version 0.1, Initial release, A. Ricke, 23 July 2009
- Version 0.2, Updated version 3.0 of the GNU General Public License and loaded code into GitHub, A. Ricke, 3 October, 2020
- Version 0.3, Updated the script to work with Python 3 and to automatically read the encoding from the file and use that encoding to import the XML file. A. Ricke 11 Oct 2020.

# CONTENTS
A listing of the MUSE XML Export contents is:

 - musexmlex.py : The Python script used to read the MUSE XML files and export a '.csv' file, suitable for import into other programs.
 - README.md : This file
 - LICENSE : A copy of the GNU General Public License. A copy is also included as part of the musexmlex.py script.

# PREPARATION

The 'musexmlex.py' script is a Python script; hence, the Python engine must be
installed before using the script. This script was verified using version 3.7.2.

See www.python.org for information about installing Python on your target 
machine.

After installation, make sure 'python3.exe' is in your system path before 
continuing.

## USE

1. Copy the  Python script to a location easily referened by your command-line 
   window.
2. Run the Python script, at the command-line, to export the ECG rhythm to a
   comma-separated value ('.csv') file. The script writes the output in 
   microvolts.
   
   For example:
   
   python musexmlex.py MUSE_FILE.xml
   
   Exports the ECG rhythm stored in the XML file to a file named 
   'MUSE_FILE.csv', assuming the following:
   
   a. The Python script 'musexmlex.py' is in the current-working directory.

   b. The file 'MUSE_FILE.xml' is in the current-working directory.

   c. Python is installed on the machine, and it is in the system path.
