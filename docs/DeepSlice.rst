**DeepSlice**
------------

.. note::
  Find DeepSlice `here <https://www.deepslice.com.au>`_ for Allen CCF and WHS. 

* *DeepSlice* performs automatic registration to the Allen CCF using Deep Convolutional Neural Networks (linear registration only). It generates a JSON file compatible with the *QuickNII* software, and can be used to automate steps 1 and 2 of the QuickNII atlas-registation process. 
* After generating a *Deepslice* JSON, it is recommended to inspect the results in *QuickNII* and to make small positional adjustments as required. 
* Use the *VisuAlign* software in a subsequent step to apply nonlinear refinements for a better fit of the atlas over the sections. 
* There is a beta-version for the Waxholm atlas of the Sprague Dawley rat. 
* At present *DeepSlice* only works for brain sections cut in the coronal plane, future versions will be compatible with sagittal and horizontal sections. 


.. tip::
  To convert an Allen CCF registration to the Kim Unified Mouse Brain Atlas use our `converter <https://www.nesys.uio.no/QuickNII/AKimBA.html>`_. 
  



