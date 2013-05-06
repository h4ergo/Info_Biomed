#WebDicom

##Giovanni Pace
##TASK: IMAGE SEGMENTATION


- - -
# Segmentation

## Problems List:

- Ingest of an image in CONTINUUM computationally not elaborable by a PC.
- An image must be simplified for the computation.
- Define a ROI (Region of Interest).
- Create a new image with only the ROI placed in.

- - -
# SOLUTIONS:
Ingest of an image in CONTINUUM computationally not elaborable by a PC.

##We need to:

- Split the image in a matrix of Dirac Pulses.
- Apply the Dirac Matrix to Image (on the Left of the image below)
- ![Sampling Array of Dirac Pulses](https://raw.github.com/h4ergo/Inf_Bio/master/PRESENTAZIONI_BIO//images_GP/sampling_array.jpg)
- FFT of every cell Indexed by the Dirac Pulse (a sample on the Right of the image).
- We have an image decomposed by Fourier Transformations.

THE IMAGE NOW IS COMPUTATIONALLY ELABORABLE

- - -
# SOLUTIONS:
An image must be simplified for the computation.

##We need to:
- Assigning a label to every pixel (assumed as a cell of the sampling matrix) that share certain visual characteristics.
- Define a pattern for recognizing of the properties of every pixel.
- Regroup every pixel that has similar properties.
- Define an approssimation pattern for simplify the regroupment.

SO YOU HAVE AN IMAGE SIMPLIFIED AS THE IMAGE BELOW (on the RIGHT)

![Sampling Array of Dirac Pulses](https://raw.github.com/h4ergo/Inf_Bio/master/PRESENTAZIONI_BIO//images_GP/simplify.jpg)

- - -
# SOLUTIONS:
Define a ROI (Region of Interest).

##We need to:
- Insert a range of color for deine WHAT WE NEED TO MARK
- Make an approssimation for defining better the ROI in the original image (GAUSSIAN BLUR METHOD)
- Cut the image and display only what we are looking for.
- Display a 8-bit image of what we are interested in.

![Sampling Array of Dirac Pulses](https://raw.github.com/h4ergo/Inf_Bio/master/PRESENTAZIONI_BIO//images_GP/thresholding.jpg)

- - -
# How it works:

![Sampling Array of Dirac Pulses](https://raw.github.com/h4ergo/prova/master/PRESENTAZIONI_BIO//images_GP/BIO-SEGM-FLUSSO_DATI.jpg)
