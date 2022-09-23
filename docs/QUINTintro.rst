**What is QUINT?**
==================

.. tip::   
   **Visit** `EBRAINS <https://ebrains.eu/service/quint/>`_ **for more information about QUINT.**

The QUINT workflow comprises a flexible suite of software designed to support atlas-based quantification of labelled features in series of histological images from mouse or rat brain. All the software are GUI-based, with no coding ability required. It generates counts and percentage coverage per atlas-region, in addition to point clouds for visualising the features in 3D. It currently supports quantification relative to the following atlases:

* Allen Mouse Brain Atlas Common Coordinate Framework version 3 (2015 and 2017) (CCFv3)
* Waxholm Atlas of the Sprague Dawley rat, version 2, 3 and 4 (WHS rat brain atlas). 

QUINT involves several defined steps: 

.. image:: images/QUINT.png
 
1. **Image preparation** using *Nutil* or another image analysis tool.
2. **Atlas-registration** with *QuickNII*, *VisuAlign* and/or *DeepSlice*. They support registration of the images to a reference atlas. Linear registration is performed using *QuickNII*, then *VisuAlign* allows refinement of the registration using non-linear methods. For coronal mouse brain sections, *DeepSlice* can automate the linear registration step.  
3. **Feature extraction** using *Ilastik* or another image analysis tool. 
4. **Quantification** with *Nutil*.
5. **Quality Control** with *QCAlign*. This is optional and supports quality control of the section images, as well as quality control of the atlas-registration. It also enables exploration of the atlas hierarchy and creation of a customized level for the quantification.
6. **Visualisation** with the *Meshview* Atlas Viewer.

**Watch our video tutorial**

.. raw:: html

   <iframe width="560" height="315" src="https://www.youtube.com/embed/n-gQigcGMJ0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
   
|

**Examples of use**
----------------------------------

QUINT supports histological sections from mouse and rat brain that have been labelled to reveal features. It works for sections cut at any angle of orientation, for complete as well as partial brain sections, and for sections affected by distortion. It can be used for:

* Cell count analysis
* To spatially characterise pathology
* Analyse tract tracing connections

**Check out the following articles that have used QUINT:**

* Ham GX, Augustine GJ. Topologically Organized Networks in the Claustrum Reflect Functional Modularization. Frontiers in Neuroanatomy. 16 June 2022. https://doi.org/10.3389/fnana.2022.901807 

* Bjerke IE, Cullity ER, Kjelsberg K, Charan KM, Leergaard TB, Kim JH. DOPAMAP, high-resolution images of dopamine 1 and 2 receptor expression in developing and adult mouse brains. Sci Data. 2022 Apr 19;9(1):175. https://doi.org/10.1038/s41597-022-01268-8

* Tocco C, Øvsthus M, Bjaalie J.G, Leergaard T.B and Studer M. Topography of corticopontine projections is controlled by postmitotic expression of the area-mapping gene Nr2f1. bioRxiv - May 2021 https://doi.org/10.1101/2021.05.10.443413
   
* Kim S, Jo Y, Kook G, Pasquinelli C, Kim H, Kim K, Hoe HS, Choe Y, Rhim H, Thielscher A, Kim J, Lee HJ. Transcranial focused ultrasound stimulation with high spatial resolution. Brain Stimul. 2021 Mar-Apr;14(2):290-300. https://doi.org/10.1016/j.brs.2021.01.002
   
* Whilden CM, Chevée M, An Seong Yeol,  Pezon Brown S. The synaptic inputs and thalamic projections of two classes of layer 6 corticothalamic neurons in primary somatosensory cortex of the mouse. J Comp Neurol. 2021 Dec;529(17):3751-3771. doi: https://doi.org/10.1002/cne.25163. Epub 2021 May 6. 
   
* McDonald MW, Jeffers MS, Filadelfi M, Vicencio A, Heidenreich G, Wu J and Silasi G. Localizing Microemboli within the Rodent Brain through Block-Face Imaging and Atlas Registration. eNeuro 16 July 2021, 8 (4) ENEURO.0216-21.2021; DOI: https://doi.org/10.1523/ENEURO.0216-21.2021    
   
* Bjerke IE, Yates SC, Laja A, Witter MP, Puchades MA, Bjaalie JG and Leergaard TB. Densities and numbers of calbindin and parvalbumin positive neurons across the rat and mouse brain. 2021, iScience.https://doi.org/10.1016/j.isci.2020.101906







