# Signal_Extraction
Larkai_Assignment<br>

#Steps to extract signal from image<br>
1. Load the image and convert it into gray scale(single channel)
2. Convert the gray image to binary image with threshold value of 90
3. To remove the salt and pepper noise, we will perform morphological operations like dilation by taking kernel size of (2,2) and number of iteration=2.
4. Now talking about main part, we will move in each column of dilated image and take median of co-ordinate values where black pixels are present i.e pixel value==0.
5. Store the value in signal file and save it in .npy format.
