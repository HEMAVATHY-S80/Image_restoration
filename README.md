The objective of this project was to enhance medical images, particularly brain MRI scans, by removing noise and converting grayscale images into color using deep learning techniques.
The two major components—image denoising and colorization—were implemented using Convolutional Neural Networks (CNNs) built in Keras.
The results were evaluated based on both quantitative metrics and visual inspection of output images.
The first part of the model focused on removing salt-and-pepper noise, which simulates data corruption commonly seen in real-world imaging due to hardware faults or transmission errors. 
Once the images were denoised, they were passed into a separate CNN trained for colorization. The model used the Lab color space, where the input grayscale image served as the L (lightness) channel, and the model predicted the a and b channels to add color.Despite the absence of true anatomical color references in MRI scans, the model generated natural-looking color images. 
The integration of denoising and colorization into a single processing pipeline significantly improved the overall output quality. 
Denoising prior to colorization ensured that the color model received clean input, thereby reducing misclassification or incorrect coloring.
