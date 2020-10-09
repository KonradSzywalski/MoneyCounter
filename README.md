# Moneycounter

The Moneycounter project is an application created in python and using The Jupyter Notebook. The application downloads a previously taken photo of coins, and then counts them and the sum of their denominations. During this project, it was required to properly process photos as well as select and use filters that allow us to extract the properties that interesting to us. My choice fell on the Skimage library. The program required the creation of a segmentation and indexation function. Progaram additionally counts the percentage of the area where the coins are located in relation to the entire photo and the Feret, Haralick and Blair-Bliss ratios.

## IMAGE PROCESSING STAGES

1. Load the image
2. Convert image to grayscale
3. Detect the edge of the coins using the Canny detector
4. Partially fill the center of the coins with binary fill holes
5. Performing a dilatation operation on partially filled coins
6. Completely fill the center of the coins with the binary fill holes
7. Performing erosion operations to separate objects
8. Performing the operations of segmentation and indexation of coins
9. Performing the watershed operation in order to return to the original shapes of the examined objects
10. Calculation of the number of objects
11. Calculation of the sum of pixels of individual objects
12. Calculating the sum of pixels of the whole image
13. Marking the specific object under study in the rectangle and assigning a nominal to it
14. Calculating the center of gravity for a specific tested object
15. Calculating the percentage of the area of ​​a specific examined object in relation to the whole image
16. Calculation of the Feret, Haralick, Blair-Bliss coefficients for a specific tested object
17. Calculating the sum of denominations for the photo loaded by us

