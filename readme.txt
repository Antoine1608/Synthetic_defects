# Synthetic Defects Creation
This repository provides tools and workflows for the generation and manipulation of synthetic defects. The main features include:

## Features
### 1. Retrieval of Support Images
* Empty Supports: Collection of empty support images.
* Conforming Supports: Collection of conforming support images.
* Non-Conforming Supports: Collection of non-conforming support images.
### 2. Pattern Extraction
* Empty Patterns: Extraction of empty patterns from empty supports.
* Defect Patterns: Extraction of defect patterns from non-conforming supports, including defect segmentation.
### 3. Creation of Empty Supports
* By combining multiple empty supports.
* By overlaying empty patterns onto non-empty supports.
### 4. Synthetic Defect Generation Workflow
A looping mechanism to generate synthetic defects:

* Random reorientation of defect patterns.
* Random selection of an empty support.
* Overlaying the defect pattern onto the empty support.
