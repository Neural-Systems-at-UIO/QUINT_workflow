**QuickNII**
--------------

.. note::
   Find full user documentation `here <https://quicknii.readthedocs.io/en/latest/>`_.
   Download `here <https://www.nitrc.org/projects/quicknii>`_.
   RRID:SCR_016854.

*QuickNII* is a tool for linear registration of (serial) 2D image data to 3D reference atlases of the brain. It currently supports the:

* Allen Mouse Brain Atlas Common Coordinate Framework version 3, 2015 and 2017.
* Waxholm Atlas of the Sprague Dawley Rat, version 2, 3 and 4. 

The registration process is semi-automated:

1. First, a few sections are registered manually by the user based on landmarks. This establishes the cutting angle of the series and the position of the sections in atlas space.  The atlas is manually scaled and rotated to achieve the best match over the sections.  
2. Next, the cutting angles and positions are propagated to the remaining sections based on the unique ID, which represents the section spacing. This happens automatically with no input from the user.
3. Finally, the registration is manually validated by the user for each section. This may involve making fine adjustments to the registration such as in-plane transformations, rotations, or small adjustments to the positions.
4. The results are exported in machine-readable formats such as JSON, XML and FLAT files. The JSON can be opened in *VisuAlign* to apply in-plane nonlinear refinements (optional). The files are also compatible with *Nutil* for quantification and spatial analysis. 




