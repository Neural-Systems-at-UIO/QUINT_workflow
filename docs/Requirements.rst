**File naming and size**
================================

All the software in the QUINT workflow have requirements for the input images:

* The images must comply with the QUINT file naming convention. It is recommended to change the file names as the first step in the QUINT workflow. This ensures that the files are compatible with *QuickNII* and *VisuAlign*, and that the output files of *QuickNII*, *VisuAlign* and *ilastik* are directly compatible with *Nutil*. 
* The image size requirements for atlas registration (using `QuickNII <https://quicknii.readthedocs.io/en/latest/imageprepro.html>`_ and VisuAlign) and feature extraction (using `Ilastik <https://quint-workflow.readthedocs.io/en/latest/Ilastik.html#preparing-images-for-ilastik>`_ or another image analysis tool) are different. It is recommended to create two image series that comply with the requirements for atlas registration (typically smaller images) and feature extraction (typically larger images). 

.. tip::
   The *Nutil* software can be used to prepare the images for analysis as it supports image transformations (downscaling, rotation, mirroring), file renaming and file format conversion. Alternative software such as *FIJI* or *Adobe Photoshop* can also be used to prepare the images.

**QUINT naming convention**
-------------------------------

.. note::

Images of brain sections from one brain are analysed together in an image series. The unique IDs are used to position the histological images in the correct anatomical order in the QUINT tools. 

* To be compatible with the tools, the image files must be named with a unique ID reflecting the serial order and spacing of the sections in the brain. The format is: _sXXX with XXX representing the section number (not restricted to three digits). Choose a starting point in the brain, either the most anterior or most posterior section, and number all the sections relative to this. 
* Do not use periods "." or spaces (" ") in the file name. This will not work. 
* As Nutil scans and detects the “_s” part of the name, the file name must not contain additional “_s” (for example "tg2345_MMSH_ss_s001.png" will not work).


**Example**

For consecutive sections: _s0001, _s0002, _s0003.

For every 2nd section: _s001, _s003, _s005

Every 10th section starting with 3rd section: _s003, _s013, _s023, _s033, etc.

.. image:: images/NamingConvention.PNG

.. tip::
   The Quantifier feature in *Nutil* uses the unique IDs to match up corresponding atlas maps, segmentations and registration information in the JSON file from *QuickNII/VisuAlign*. While not recommended, it is possible to bypass the naming convention in *Nutil* using Regular Expressions (RegExp) as long as there is a consistent naming convention across the files. For more information see the “Help” button in the *Nutil* GUI or contact user support.

