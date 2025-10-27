**File naming and size**
================================

All the software in the QUINT workflow have requirements for the input images:

* The images must comply with the QUINT file naming convention. It is recommended to change the file names as the first step in the QUINT workflow. This ensures that the files are compatible with *QuickNII* and *VisuAlign*, and that the output files of *QuickNII*, *VisuAlign* and *ilastik* are directly compatible with *Nutil*. 
* The image size requirements for the atlas registration step (using `QuickNII <https://quicknii.readthedocs.io/en/latest/imageprepro.html>`_ and VisuAlign) and the feature extraction step (using `Ilastik <https://quint-workflow.readthedocs.io/en/latest/Ilastik.html#preparing-images-for-ilastik>` or another image analysis tool)_ are different. It is recommended to create two image series that comply with the respective requirements for atlas-registration (typically smaller images) and feature extraction (typically larger images). 

.. tip::
   The *Nutil* software can be used to prepare the images for analysis as it supports image transformations (downscaling, rotation, mirroring), file renaming and file format conversion. Alternative software such as *FIJI* or *Adobe Photoshop* can also be used to prepare the images.

**QUINT naming convention**
-------------------------------

* Add a unique ID to the file names of the images reflecting the serial order and spacing of the sections. The format is: _sXXX with XXX representing the section number (not restricted to three digits). As *QuickNII* propagates the registration using these numbers, it is important they reflect the order and spacing of the sections (the direction does not matter, e.g. for coronal sections, can be either from anterior to posterior or posterior to anterior). 
* Do not use periods "." or spaces (" ") in the file name. This will not work. 
* As Nutil scans and detects the “_s” part of the name, the file name must not contain additional “_s” (for example "tg2345_MMSH_ss_s001.png" will not work).

Example for consecutive sections: _s0001, _s0002, _s0003.

Example for every fourth section starting with the third section: _s003, _s007, _s0011. 

.. image:: images/NamingConvention.PNG

.. tip::
   The Quantifier feature in *Nutil* uses the unique IDs to match up corresponding atlas maps, segmentations and registration information in the JSON file from *QuickNII/VisuAlign*. While not recommended, it is possible to bypass the naming convention in *Nutil* using Regular Expressions (RegExp) as long as there is a consistent naming convention across the files. For more information see the “Help” button in the *Nutil* GUI or contact user support.

