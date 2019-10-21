# Digital-Image-Processing
Implementing many Digital Image Processing Operations in MATLAB covering the syllabus of B.Tech(CSE)

# 1.	Compute the following quantities:
(i) 25/(25-1) ,     (1-1/25)-1 ,     (√5-1)/( √5+1)2	

(ii) e3 ,     ln(e3) ,     log10(e3) ,     log10(105) ,     eπ√163

(iii)sin π/6 ,     cos π ,     tan π/2 ,     sin2 π/6  + cos2 π/6 

(iv) (1+3j)/(1-3j) ,     ej π/4 ,     e π/2*j ,     e π/2j

# 2.	Compute the y-coordinates of a line with slope, m=0.5 and the intercept, c = - 2 at the following x-coordinates.

x = 0, 1.5, 3, 4, 5, 7, 9 and 10.

Use equation y=mx + c.

# 3.	Create a vector, t with 10 elements: 1,2,3……10 and compute the following:
y= (t-1)/(t+1),     z= (sin (t2) )/ t2

# 4.	All points with coordinates x = r cos θ  and  y = r sin θ , where r is a constant, lie on a circle with radius r. Create a column vector for θ with the values 0, π/4, π/2, 3π/4, π and 5π/4, 3π/2, 7π/4, 2π. Compute x, y and  x2 + y2for every value of  θ and display them as column vectors.Take r=2.

5.	Plot for x and y in Q2 & Q4. Give suitable title of the plots. Also annotate the axes in both plots. Try the command axis(‘equal’) and comment. Mark the points by ‘o’. Both plots must be displayable simultaneously.

6.	Modify Q4 by taking the interval for  θ as π/12 and then plot the circle.

7.	Write a script file to print table of 5.

8.	Write a script file to print first twenty prime numbers.

9.	Write a function that gives the greatest number of three given numbers.

10.	Write a function that gives sum and product of two given numbers.

11.	(i) A 2D function of order 4X4 has all the elements as one. Find the DFT of the function and also apply the IDFT to get the function/matrix back.
Use dftmtx( )  to get the kernel.
(ii)Use directly fft2( ) and ifft2( ) to obtain the final result.

12.	Let f=[1 2;2 1].
(i) Find the DCT of the function and also apply the IDCT to get the function/matrix back.
     Use dctmtx( )  to get the kernel.
(ii)Use directly dct2( ) and idct2( ) to obtain the final result.

13.	A 2D matrix of order 8X8 has all the elements as one. Find the Walsh-Hadamard transform of the matrix. Also get the matrix back.
Use fwht( ) and  ifwht( ).

14.	Use the following code to create a gray-scale image and save it using imwrite( ).
image=zeros(256);  % or use image=ones(256)
[m n]=size(image);
for i= 110:140
   for j=110:140
      image(i,j)=255;  % or use image(i,j)=0
   end	
end

15.	Illustrate imread( ) and imshow( ) to read and display the image created in the above question. Also try imadjust() and imresize().

16.	Create two different images somewhat similar to the one as described in Q14 and apply the following arithmetic and logic operators: + , - , *, / , AND, OR, XOR, NOT.
Make the program interactive by asking the user to enter the choice for a particular operation. For this use input( ). Display the resultant image.
Before performing the logical operations convert the images into their corresponding binary images using the function logical().

17.	Prove the convolution property. As per this property the convolution of two matrices in spatial domain is equal to multiplication of the transformed matrices in frequency domain.
Hint: Create two images somewhat similar to the one as described in Q 14. Take the convolution of them using conv2( ).Then take the array product of the two transformed matrices. Get back to Spatial domain. Use fftshift() to shift the origin to the center.   Display the convolution and the multiplication using imshow( ). 

18.	The rotation property states that if a function is rotated in spatial domain, its Fourier transform also rotates by an equal amount. Prove this property by creating an image somewhat similar to the one as described in Q 14. Rotate the image by 45 degrees. Display the two images along with their Fourier Transforms in one figure.  Give the titles for the four subplots as “Original Image”, ”Rotated Image”, “Original Image Spectrum” and “Rotated Image Spectrum”. Use imrotate( ) and subplot( ).
            Use “mat2gray(log(1+abs(fftshift(fft2(f)))))” to display the transformed image, f is the   
            image.

19.	Perform PCA on the following data set and find out the transformed data.
       X            Y         
    2.5000    2.4000
    0.5000    0.7000
    2.2000    2.9000
    1.9000    2.2000
    3.1000    3.0000
    2.3000    2.7000
    2.0000    1.6000
    1.0000    1.1000
    1.5000    1.6000
    1.1000    0.9000
Use pca( ).

20.	Read a grey-scale image and perform histogram equalization. Display the following in one figure.
i)	Original image
ii)	Plot of  Original histogram 
iii)	Image after histogram equalization
iv)	Plot of equalized histogram.
Use histeq(), imhist(), subplot(), etc

21.	Read a gray-scale image and convert it into binary image using hard thresholding. Make  
            the threshold value as a user-defined parameter. Take different threshold values at
            different runs and observe the results.
            Use input() to input the threshold value.

22.	Read an image, convolve the image with the 3 X 3 mask as shown

     1
     9	
X	1	1	1
		1	1	1
		1	1	1
and show that it perform averaging operation which results in blurring the image. Also analyze the impact of increasing the size of mask to 5 X 5 as shown




  1
 25	


X	1	1	1	1	1
		1	1	1	1	1
		1	1	1	1	1
		1	1	1	1	1
		1	1	1	1	1
        
23.	Read an image and then corrupt the image by salt-and-pepper noise and Gaussian noise. Then apply an averaging filter of size 3 X 3 and 5 X 5 to this corrupted image. Comment on the result obtained.
Use imnoise()

24.	Read an image, then corrupt the image using ‘salt-and-pepper’ noise. Now apply a 3 X 3 averaging filter and median filter. Comment on the result.
Use medfilt2().

25.	Read an image and filter it with the following Laplacian second-order derivative operator for sharpening
                    

     
     	
	-1	-1	-1
		-1	  8	-1
		-1	-1	-1

26.	Read an image and apply Ideal low-pass filter. Display both the images. Also display the 2D and 3D views of the filter.

27.	Read an image and apply Ideal high-pass filter. Display both the images. Also display the 2D and 3D views of the filter.
Use surf() for 3D view.

28.	Read an image and apply Butterworth low-pass filter. Display both the images. Also display the 2D and 3D views of the filter.

29.	Read an image and apply Butterworth high-pass filter. Display both the images. Also display the 2D and 3D views of the filter.


30.	Read an image and apply Gaussian low-pass filter. Display both the images. Also display the 2D and 3D views of the filter.

31.	Read an image and apply Gaussian high-pass filter. Display both the images. Also display the 2D and 3D views of the filter.

32.	Read an image and apply band-pass filter. Display both the images. Also display the 2D and 3D views of the filter.

33.	Read an image and apply band-reject filter. Display both the images. Also display the 2D and 3D views of the filter.

34.	Read an image and detect edges using different edge detectors like Robert, Sobel, Prewitt, Log, Canny.
Use edge( ).

35.	
     






