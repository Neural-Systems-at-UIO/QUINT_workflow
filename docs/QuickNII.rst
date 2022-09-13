**QuickNII**
--------------

QuickNII is a tool for spatial registration of (serial) 2D image data to 3D reference atlases of the brain. It currently supports:

* the Allen Mouse Brain Atlas, version 3, 2015 and 2017.
* the Waxholm Atlas of the Sprague Dawley Rat, version 2, 3 and 4. 

The registration process is semi-automated, with three parts:

1. A few sections are registered manually based on the appearance of landmarks in the sections. This establishes the probable cutting angle of the series and the position of the sections in 3D atlas space. The atlas-planes are manually scaled and rotated to achieve the best match over the sections.  
2. The cutting angles and positions are propagated to the remaining sections based on the section spacing (reflected in the unique ID). This happens automatically with no input from the user.
2. The registration is manually validated by the user. This may involve making fine adjustments to the registration such as in-plane transformations and rotation or small adjustments to the positions.



A linear registration is first performed using QuickNII, then VisuAlign allows refinement of the registration using non-linear methods.
