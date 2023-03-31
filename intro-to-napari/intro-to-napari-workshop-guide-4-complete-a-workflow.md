# Segmentation workflow

This workshop takes you through the following topics with some hands on exercises: 

* [Installing and Opening/Closing napari](intro-to-napari-workshop-guide-1-install-napari.md) - 15 minutes  
* [Explore the viewer](intro-to-napari-workshop-guide-2-explore-the-viewer.md) - 15 minutes  
* [Plugins](intro-to-napari-workshop-guide-3-plugins.md) - 15 minutes  
* This guide (Complete a workflow) - 15 minutes
* [Jupyter notebooks and napari](intro-to-napari-workshop-guide-5-jupyter-notebooks-and-jupyter-lab.md) - 30 minutes
* [Resources](intro-to-napari-workshop-guide-6-resources.md)  

This is a segmentation workflow:

* Install [PartSeg](https://www.napari-hub.org/plugins/PartSeg) and [napari-segment-blobs-and-things-with-membranes](https://www.napari-hub.org/plugins/napari-segment-blobs-and-things-with-membranes).  
**Note:** If you do not see PartSeg Widgets after installing PartSeg, close napari and reopen it.   
* Download the [Sample Data](https://github.com/chanzuckerberg/napari-segmentation-workshop/raw/main/content/workflow/images/cells_gh2ax.tif) and complete this [lesson written by Kasia Kedziora](https://chanzuckerberg.github.io/napari-segmentation-workshop/workflow/partseg.html).

    **Note:** The lesson lists a different version of napari (0.4.15) than the version you are using (0.4.17). However, the steps are the same.

   **Note:** The following parameter settings are referred to in the lesson by Kasia Kedsiora. They are listed here for your convenience.  

    * PartSeg: ROI Mask Extraction parameters:
        * Median filtering (r = 2)
        * Thresholding ‘Otsu’
        * Opening (r = 5)
        * Fill holes (r = 100)
        * Size restriction (>400)
        * Connect by sides  
        * Convex hull (r = 1)  

    * Napari-segment-blobs-and-things-with-membranes: Gaussian Laplace filter  
    * PartSeg: ROI analysis extraction parameters:
        * Mask (nuclei):
        * Manual Threshold (-2)
        * Size restriction (>3)
        * Connect by side

The final guide in this workshop is [Jupyter notebooks and napari](intro-to-napari-workshop-guide-5-jupyter-notebooks-and-jupyter-lab.md). It takes about 30 minutes to complete.