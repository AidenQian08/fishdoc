Introduction
============

Project Context
---------------

The 4D Nucleome Project
~~~~~~~~~~~~~~~~~~~~~~~

The 4D Nucleome (4DN) project is a pioneering research initiative aimed at understanding the dynamic three-dimensional (3D) architecture of the nucleus in space and time (the fourth dimension). This large-scale effort seeks to map how chromatin (the material that makes up chromosomes) is organized within the nucleus of cells, and how this organization influences gene expression and cellular function. The project brings together interdisciplinary research groups to develop innovative methods for imaging, modeling, and analyzing chromatin at various scales, providing valuable insights into how the genome is regulated in both normal development and disease states.

Fish-Omics and the FOF-CT Format
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Fish Omics is a collection of techniques designed for imaging chromosomes using Fluorescence In Situ Hybridization (FISH) to capture spatial information about chromatin. The **4DN FISH Omics Format - Chromatin Tracing (FOF-CT)** is a standardized format developed to support the storage and exchange of results from these imaging experiments. While this format has proven essential for the exchange of chromosome imaging data, it can be cumbersome to search through and requires significant hardware resources due to its large file size.

FOF-CT CSV Files and Key Columns
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

The FOF-CT format consists of several key CSV tables, each serving a specific purpose in organizing chromatin tracing data. The **Core Table** is mandatory and contains the essential data required for chromatin mapping. The **RNA Table** is used for RNA FISH experiments, while the **Spot Table** provides quality metrics for the spots. The **Bio Table** stores biological properties associated with each spot, and the **Demultiplexing Table** is used for multiplexed FISH experiments.

Additional tables include the **Trace**, **Cell**, **Sub Cell**, and **Extra Cell** tables, which document properties related to traces and cellular structures. The **Mapping Table** ties together spatial data of cells and sub-cellular features.

The FOF-CT format includes several key columns that are essential for organizing and querying chromatin tracing data:

- **Spot ID**: This unique identifier corresponds to individual spots detected in FISH experiments, which represent specific chromatin regions.
- **Trace ID**: This column tracks individual traces, grouping multiple spots that belong to the same chromatin trace.
- **Cell ID**: This identifier is used to link data points to specific cells, allowing the study of chromatin organization within individual cells.
- **Chrom Start**: This column represents the starting position of a chromatin region on a chromosome, facilitating the mapping of chromatin locations.

These columns play a crucial role in organizing the data and enabling efficient queries within the datasets.

For a more detailed guide on the FOF-CT file format, visit `this website <https://fish-omics-format.readthedocs.io/en/latest/index.html>`_.


Project Goals
-------------

Phase 1: Python Parser for FOF-CT Files
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

In this phase, we focus on building a Python parser that allows users to input their FOF-CT CSV files. This parser merges and compresses the files into a new, more efficient format called the **.FISH file**, reducing the hardware space requirements without sacrificing data integrity.

Phase 2: JavaScript Query and Filter Program
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Once the data is compressed, we develop a JavaScript-based program to query and filter through the .FISH files efficiently. This phase ensures that the compressed data remains easy to navigate, even with large datasets.

Phase 3: User Interface for Data Input and Visualization
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

In the final phase, we provide users with a fully interactive user interface. This interface allows them to:

1. Input their own .FISH files or use pre-processed datasets.
2. Visualize the data with a 3D model alongside additional informative tables.
3. Set their queries using a function bar, linked directly to the JavaScript query program from Phase 2.

Through these steps, we aim to simplify the management and visualization of FISH Omics data, enhancing both usability and performance.
