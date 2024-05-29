**Nutil**
------------


.. note::
   Full `Nutil user documentation <https://nutil.readthedocs.io/en/latest/>`_. (RRID: SCR_017183).
   `Download here <https://www.nitrc.org/projects/nutil>`_.
   
.. Warning::

   Nutil v0.7.0 and v0.8.0 are stable and validated with multiple ground truth datasets. It is not recommended to use Nutil v0.4.0 - v0.6.0 as they contain bugs that lead to incorrect results in some of the reports: see the `release notes <https://nutil.readthedocs.io/en/latest/release.html>`_ for more information. 

   
*Nutil* is a pre- and post-processing toolbox for histological images. It is an integral part of the QUINT workflow, enabling image transformations, file format conversion and renaming of files in order to prepare images for the *QuickNII* and *ilastik* software. It also supports the final quantification step in the workflow. *Nutil* has four features: 

1. **TiffCreator**: convert JPEG, PNG and normal TIFF images to tiled TIFF format.

2. **Transform**: rename, rotate, resize and compile thumbnails of large tiled TIFF images (typical microscopy output format).

3. **Resize**: for resizing JPEG/PNG images with output in PNG format.

4. **Quantifier**: for the batch extraction, quantification and spatial analysis of labelling in mouse or rat brain sections.

For detailed instructions on how to use Nutil and analyse results, please go to the Nutil `user documentation <https://nutil.readthedocs.io/en/latest/>`_.




