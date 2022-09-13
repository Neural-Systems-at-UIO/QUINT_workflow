**Preparing the images**
==========================

All the software in the QUINT workflow have image input requirements:

* The file naming convention applies to all the software.
* The image size requirements differ for the QuickNII and ilastik software. Generate two separate series that comply with the respective requirements.
* The Nutil software can be used to prepare the images for QuickNII and ilastik since it supports image transformations, renaming of files and file format conversion. 

**QUINT naming convention**
-------------------------------

Add a unique ID to each image that reflects the serial order and spacing of the sections. The format is: _sXXX..., with XXX.. representing the section number (not restricted to three digits). For example, for three consecutive sections: tg2345_MMSH_s0001.png, tg2345_MMSH_s0002.png, tg2345_MMSH_s0003.png. 

.. tip::
   It is recommended to change the file names as the first step in the QUINT workflow. This ensures that the files are compatible with QuickNII and VisuAlign, and that the output files of QuickNII, VisuAlign and ilastik are directly compatible with Nutil Quantifier. 


**Preparing images for QuickNII**
---------------------------------

**Preparing images for ilastik**
--------------------------------




