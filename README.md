# image-denoise
Based on 'n' numbers of matrices, create an average matrix of them (image denoise).

## Reading data
File with data is given in a .txt file.
First line is the number of rows and columns in matrices (their size) separated by 'x'.
Following lines are matrices separated by spaces, one line for each matrix.
If the calculations succeed, script appends the result at the end of the file.

## Runnning program
Running the program displays in the terminal bunch of useful information for the calculations
such as average, standard deviation and error for each pixel calculated.

The program can run in two modes:
+ **standard** - where the images are assumed to be of the same quality.
+ **weighted** - where each image was created differently.

To run in the _weighted_ mode, append `-w` flag and the path to the file
with weights (yes, weights must be calculated by hand).

To use the script, type: `python image_denoise.py path/to/matrices_file.txt [-w path/to/weight_file.txt]`
