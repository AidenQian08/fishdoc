Using the User Interface
========================

Home Page
---------

The home page provides various tools to help you navigate and get started with the application.

Guided Tour
~~~~~~~~~~~

To begin the guided tour of the application, click on the orange 'Guided Tour' button.

.. image:: path/to/guided-tour-button-image
   :alt: Guided Tour Button

Video Tutorial
~~~~~~~~~~~~~~

To access the video tutorial, scroll down to the bottom of the home page.

.. image:: path/to/video-tutorial-image
   :alt: Video Tutorial

Import Page
-----------

On the import page, you can either upload your own data by importing a `.FISH` file or choose from a selection of pre-processed datasets available on our website.

Uploading Local File
~~~~~~~~~~~~~~~~~~~~

To upload a file from your local machine, click the 'Choose File' button, followed by 'Upload File'. Once the upload is successful, a confirmation message 'Upload Successful' will appear. If the message does not appear, the file upload was unsuccessful. Please try again.

.. image:: path/to/local-file-upload-image
   :alt: Local File Upload

Input File Path
~~~~~~~~~~~~~~~

Another option for uploading data is through providing a file path. Similar to the local file upload, after a successful upload, the message 'Import Successful' will be displayed. If the message does not appear, please try again.

.. image:: path/to/file-path-upload-image
   :alt: File Path Upload

Using Pre-Existing Data
~~~~~~~~~~~~~~~~~~~~~~~

If you wish to view pre-existing datasets already available within the application, you can select from the list of processed datasets available on the import page.

.. image:: path/to/pre-existing-data-image
   :alt: Pre-existing Data

Visualization Page
------------------

The visualization page offers powerful tools to interact with and analyze your data. It is divided into three main sections: the Function Bar on the left, the 3D Visualization on the right, and the Additional Information Tables at the bottom.

Function Bar
~~~~~~~~~~~~

The function bar allows you to customize and manipulate the visualization of your data. Below are the key features:

Chromosome Filter
^^^^^^^^^^^^^^^^^

Use the 'Chromosome' dropdown to filter the data based on specific chromosomes.

.. image:: path/to/chromosome-filter-image
   :alt: Chromosome Filter

Filter Options
^^^^^^^^^^^^^^

The filter dropdown allows you to refine your data based on specific parameters.

1. **Sequenced Data**  
   The 'Sequenced' filter option includes the Spot_ID and Chromosome Start columns. You can filter data using sliders for these columns.

2. **Non-sequenced Data**  
   The 'Non-sequenced' filter option includes the Trace_ID and Cell_ID columns. Filtering is performed through input boxes and dynamic lists that update as data points are added or removed.

3D Visualization
~~~~~~~~~~~~~~~~

The 3D Visualization graph displays the spatial (X, Y, Z) coordinates of each data point within your selected query range. Each trace is highlighted with a distinct color. This graph, developed using Plotly, offers various interactive features, such as hovering over data points to display information like Spot ID or Trace ID.

.. image:: path/to/3d-visualization-image
   :alt: 3D Visualization

Additional Information Tables
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

The additional tables at the bottom of the visualization page present detailed information corresponding to the data points. To retrieve information, select a point from the 3D Visualization and enter either the Spot_ID or another relevant identifier into the input field. After clicking 'Search', if a matching data point is found, a data table will be displayed. If no matching data point is found, no table will be generated.

.. image:: path/to/additional-info-tables-image
   :alt: Additional Information Tables