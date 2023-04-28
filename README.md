# rsdoc-to-sat
Convert DesignSpark Mechanical [DSM] rsdoc file to sat file which can be loaded into 3D Modellers that can open SAT files
<br>
<br>

## Installation
Install [DSM] v1,2,..,5 (it provides SabSatConverter.exe). Install [python3].
<br>
<br>

## Running The File Converter Method 1
1. Download this ZIP, then UnZIP it 

    <img width="300" alt="image" src="https://user-images.githubusercontent.com/26157143/235037868-287ab373-26bd-457d-9445-a6bff266984e.png">

2. Copy and paste the .rsdoc file into the same directory as the UnZIP file.

3. Open CMD that has Path to python.exe recognised (either native installation or conda environment). In the cmdline window, `cd`  to the same directory as [2].

    <img width="850" alt="image" src="https://user-images.githubusercontent.com/26157143/235039456-0c8f8d38-b6ee-4a1d-b4f8-2e3c1111db77.png">

4. For Windows Machine, drag and drop the .BAT script into the CMDline window, and press enter. Voila. 

    <img width="850" alt="image" src="https://user-images.githubusercontent.com/26157143/235039614-03a3526e-68f8-4b6e-8e4f-d05c79a01f79.png">

5. .sat file(s) will appear in the same directory as rsdoc file(s).
<br>

### Important Note.
6. If you see multiple .SAT files generated for the same design; it was caused by the Assembly file belongs to 1 Parent Design / Assembler. If you like them merged again, 

   1. You can either merge the .SAT files again using the same origin or 
   
   1. in DSM remove all assembly information and just retain the Solids

<br>
<br>

## Running The File Converter Method 2
1. Download this ZIP, then UnZIP it 
2. Copy and paste the .rsdoc file into the same directory as the UnZIP file.
3. Open CMD that has Path to python.exe recognised (either native installation or conda environment). In the cmdline window, `cd`  to the same directory as [2].
4. Run this command below in the cmdline window

````
python rsdoc-to-sat.py <rsdoc file>
````



.sat file(s) will appear in the same directory as rsdoc file(s).

<br>
<br>

## Credits:

[dsm]:http://www.rs-online.com/designspark/electronics/eng/page/mechanical
[python3]:http://python.org/

code original source: [arekm / maven.pl](https://github.com/arekm/rsdoc-to-sat)
