**QuickNII**
--------------

.. note::
   `QuickNII user manual and download information <https://quicknii.readthedocs.io/en/latest/>`_. RRID:SCR_016854.

*QuickNII* is a tool for linear registration of (serial) 2D image data to 3D reference atlases of the brain. It currently supports the:

* Allen Mouse Brain Atlas Common Coordinate Framework version 3, 2015 and 2017.
* Waxholm Atlas of the Sprague Dawley Rat, version 2, 3 and 4. 
* `New Unified Mouse atlas from the KIM lab <https://www.ebrains.eu/news-and-events/new-unified-mouse-atlas-from-the-kim-lab-is-now-available-in-the-ebrains-quicknii-image-registration-tool/>`_.
* `Developmental Mouse Brain Atlas for ages P4-P56 (DeMBA) <https://www.ebrains.eu/news-and-events/4d-atlas-representing-mouse-brain-development-from-adolescence-to-adulthood-now-available-on-ebrains>`_
* Some other atlases have been made available in our tools by external users (contact us at EBRAINS support to find out more).

The registration process is semi-automated:

1. A few sections are registered manually by the researcher using anatomical landmarks. This establishes the cutting angle of the image series and the position of the sections in atlas space. The atlas is manually scaled and rotated to achieve the best match over the sections.  
2. The cutting angles and positions are automatically propagated by QuickNII to the remaining sections using the unique section IDs, which represent the section spacing. This happens automatically with no input from the user.
3. The registration is manually validated by the user for each section. This may involve making fine adjustments to the registration such as in-plane transformations, rotations, or small adjustments to the positions.
4. The results are exported in machine-readable formats such as JSON, XML and FLAT. The JSON can be opened in *VisuAlign* to apply in-plane nonlinear refinements (optional). The files are also compatible with *Nutil* for quantification and spatial analysis. 




