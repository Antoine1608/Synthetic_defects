# Synthetic Defects Creation
Generation of synthetic images based on images of Conform and Not Conform products using openCV

## Step 1 : collecting images
	* The images consist in a view of an automotive part where a tape is pasted on a specific spot. The tape has a rectangular shape and is white on te images.
	* Sometimes, the tape is pasted sideways or two tapes are pasted instead of one :
	* Conform and Not conform images are collected in two specific folder : "C" for C images and "NC" for NC images. A third folder "empty" contains images where the tape is absent like this one :

## Step 2 : extracting windows of interests
	* We extract empty windows from the images in the "empty" folder. We will superpose these empty windows on images to use in further steps.

## Step 3 : extracting tabs
	* We extract Conform and Not Conform tabs using the GrabCut method from openCV on C and NC images

## Step 4 : creating synthetic images without tabs
	* We superpose empty windows on images (C and NC)
	* To increase the number of synthetic images we combine them together

## Step 5 : creating C synthetic images
	* We superpose Conform tabs on empty images

## Step 6 : creating NC synthetic images
	* We use a combination of methods to create NC images by :
		* superposing NC tabs on empty images
		* superposing misoriented C tabs on empty images
		* superposing a misoriented C tab on a C image

## Step 7 : creating a train folder
	* We create a train folder withe a C and a NC subfolder where we put 1000 C and NC images. 
	* This way we have a balanced dataset to use for image classification
	
