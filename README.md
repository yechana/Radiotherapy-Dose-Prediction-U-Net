# U-Net

The contents of this archive are files needed to build and train the U-Net model with 3D convolutions, and to make needed visualizations. To run the code, you need the data provided by the Open-KBP challenge, which can be fetched from [here](https://github.com/ababier/open-kbp/tree/master/provided-data). The provided-data folder needs to be in the same directory as the code files. The files found in provided_code directory were provided by the Open-KBP challenge to help with reading in the data.

## U-Net Main

This is the code that reads in all of the data, defines the U-Net model, and trains it. It also gets the test dose scores (MAE) and makes visualizations of the CT image and ground-truth or prediction dose (relies on [mayavi](https://github.com/enthought/mayavi)). 


## U-Net Learning Curves

This auxiliary code draws the learning curves of some of the configurations tested. It needs the pickled loss files included in the archive.

## U-Net Data Visuals
This auxiliary code fetches a sample patient from the training data and draws its contoured CT image as well as their ground-truth dose (relies on [mayavi](https://github.com/enthought/mayavi)).