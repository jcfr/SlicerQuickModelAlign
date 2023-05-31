# QuickAlign

This is a 3D Slicer extension that allows for rapid alignment and comparison (visual & metric) of two 3D models using ALPACA's point-cloud based alignment capabilities.

It is freely usable, without any restrictions.

<img width="983" alt="Screen Shot 2023-05-31 at 2 50 54 am" src="https://github.com/seanchoi0519/SlicerQuickAlign/assets/33897705/56f2cdb4-c033-4156-853b-6ff4efbe1978">


## Installation

- Download and install a latest stable version of 3D Slicer [https://download.slicer.org]
- Start 3D Slicer application, open the Extension Manager (menu: View/Extension manager)
- Install QuickAlign extension

## Tutorial
- Start 3D Slicer
- Switch to "Quick Align" module: if first time opening the module, wait for additional installations to complete 
- Load the two 3D model files (supports .ply format only - for now) being compared on the left tab
- Click 'Load Models': The two models will be reduced to point-cloud based representation, ready for alignment
- Click 'Align Models': Wait about 5 seconds for software to run alignment & analysis
- Inspect results: 

### User Interface Overview

<img width="852" alt="Screen Shot 2023-05-31 at 3 00 13 am" src="https://github.com/seanchoi0519/SlicerQuickAlign/assets/33897705/5c2f7fdc-0461-4caf-a2ea-169ea3f7d2d5">

## Visualize and Analyze results
There are 3 display modes available to visualize and analyze the comparison results
### 1. Normal Mode (Default)

<img width="633" alt="Screen Shot 2023-05-31 at 2 44 28 am" src="https://github.com/seanchoi0519/SlicerQuickAlign/assets/33897705/b0ae5efa-1cf2-465f-aa62-db7723ae33e2">

- The advantage of this mode is that it allows the most simple visualization of the aligned models.
To enable this display mode, press "1" on keyboard

### 2. Wireframe Mode

<img width="882" alt="Screen Shot 2023-05-31 at 2 26 38 am" src="https://github.com/seanchoi0519/SlicerQuickAlign/assets/33897705/7e96ed5c-c24f-45c9-9f71-3fd379fc2ad9">

- The advantage of this display mode is that it allows visualization of the internal layers and structures of the aligned models.
To enable this display mode, press "2" on keyboard

### 3. Colour Map Mode

<img width="509" alt="Screen Shot 2023-05-31 at 2 26 45 am" src="https://github.com/seanchoi0519/SlicerQuickAlign/assets/33897705/9f337404-55ba-49ce-9403-6368d2ce0665">

- The advantage of this display mode is that it visually highlights areas of difference between the aligned models in colors (Red/Blue).


Colour 'Red' - highlights areas in the 'Prepared" model' that are excess or "under-prepared" compared to the ideal.
Colour 'Blue' - highlights areas in the "Prepared" model that are deficient or "over-prepared" compared to the 'Ideal' model.

To enable this display mode, press "3" on keyboard

### Animation

Note that by default, there is a live animation that goes back and forth between the two models to aid in visualization.
To start or stop the animation, press "spacebar" on keyboard

## Advanced Settings

### Error Tolerance

- Error tolerance (mm) can be adjusted under "advanced settings" header in the left tab.
The concept of error tolerance is that it takes into account possible micro-errors in the alignment, or during the scanning & capturing of 3D data. In the colour map mode, only differences exceeding this error tolerance will be highlighted in color (red/blue). The initial value is set to 0.15mm (recommended).

## Publications

## Acknowledgments





