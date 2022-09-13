**Preparing the images**
==========================

All the software in the QUINT workflow have requirements for the input images:

* The file naming convention applies to all the software.
* As the image size requirements for `QuickNII <https://quicknii.readthedocs.io/en/latest/imageprepro.html>`_ and `Ilastik <https://nutil.readthedocs.io/en/latest/Ilastik.html#preparing-the-images-for-ilastik>`_ differ, generate two separate series that comply with the respective requirements. 
* The Nutil software can be used to prepare the images since it supports image transformations, renaming of files and file format conversion. Alternative software such as FIJI or Adobe Photoshop can also be used. 

.. tip::
   It is recommended to change the file names as the first step in the QUINT workflow. This ensures that the files are compatible with QuickNII and VisuAlign, and that the output files of QuickNII, VisuAlign and ilastik are directly compatible with Nutil Quantifier. 



**QUINT naming convention**
-------------------------------

* Add a unique ID to each image that reflects the serial order and spacing of the sections. 
* The format is: _sXXX with XXX representing the section number (not restricted to three digits). 

For example, for consecutive sections: _s0001, _s0002, _s0003

.. image:: images/NamingConvention.PNG



