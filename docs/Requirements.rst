**Preparing the images**
==========================

All the software in the QUINT workflow have input requirements for the images:

* The file naming convention applies to all the software.
* The image size requirements differ for the QuickNII and ilastik software. Generate two separate series that comply with the respective requirements.
* The Nutil software can be used to prepare the images since it supports image transformations, renaming of files and file format conversion. Alternative software such as FIJI or Adobe Photoshop can also be used. 

**QUINT naming convention**
-------------------------------

Add a unique ID to each image that reflects the serial order and spacing of the sections. The format is: _sXXX..., with XXX.. representing the section number (not restricted to three digits). For example, for three consecutive sections: tg2345_MMSH_s0001.png, tg2345_MMSH_s0002.png, tg2345_MMSH_s0003.png. 

.. tip::
   It is recommended to change the file names as the first step in the QUINT workflow. This ensures that the files are compatible with QuickNII and VisuAlign, and that the output files of QuickNII, VisuAlign and ilastik are directly compatible with Nutil Quantifier. 


**Preparing images for QuickNII and ilastik**
-----------------------------------------------

As the image size requirements for QuickNII and ilastik differ, generate two separate series that comply with the respective requirements. 

`QuickNII <https://quicknii.readthedocs.io/en/latest/imageprepro.html>`_ requirements. 
`Ilastik <https://nutil.readthedocs.io/en/latest/Ilastik.html#preparing-the-images-for-ilastik>`_ requirements.



