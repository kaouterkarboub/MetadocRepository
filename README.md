# MetadocRepository
This repository is a go through steps for Metadoc Updated Solutions
This repository contains two different updates for Metadoc Solutions: 

1. Full Body Posture assessment
2. Seated person assessment based on videos

The above solutions contain the following docs for each: 
a. Code for the solution 
b. Resources to run code (from the original format to used format) 
c. doc file to explain how to run the code and use the resources. 
d. Results after running code

Steps to Run a code: 

Go to Link : https://colab.research.google.com/XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX

Then upload the resources to your workspace as mentionned: 

![image](https://user-images.githubusercontent.com/37115711/228078180-8d166ca5-527f-432c-b6f1-49fe814f2b4a.png)


Once you ve uploaded the resources, make sure the ID of the resource is same as mentioned in code, run cells sequentially. 

Note: The results of each solution (either videos or spreadsheet are accompanied with docs. 

YOU CAN REPRODUCE THE RESULTS. 

1. Full Body Assessment: 

1.1. Images processing and splitting: 
Training data : over 600 images from : 
Testing data : 50 images (with Dr. Armia’s score for validation : reference). 

Step 1: dowload picture link above. 
Step 2: filer the images, here comes a really problematic thing, I noticed that there are images such as (see link) : https://drive.google.com/drive/folders/1qLNkTrD-voTkHSPuNs9QV6AkhTNWxpIG?usp=sharing 
Step 3: Convert all png files to jpg files. 
Step 4: Rename all photos to have a unified name : “Picture{i}.jpg” 
******************First Version: ********
Code : 
https://colab.research.google.com/drive/1VJWZgVlMg0oHpgV6gptGl2Rorjd5IUtc?usp=sharing

1.2. Used resources: https://drive.google.com/drive/folders/1UCeoxSmmm7CslrgpKquCVKtiJZDZeJ-z?usp=sharing 

1.3. Results: 
spreadsheet that contains results after running of : 
Landmarks before normalization 
Landmarks corrdinates after normalization
A photo of the person of course a standing still position
Parts of the body taken into account
Calculated angles using our version
Corresponding scores from Dr.Armia’s assessment. 
Pictures of landmarks in a 3 dimensional orientations.
File:https://docs.google.com/spreadsheets/d/1KW78wckjBiyydwk1ba1V4wc9LHsNEl7LF9o1g2vKXoU/edit?usp=sharing

A collected dataset where only labels of body parts, angles and scores are taken into account: 
File: [dataset](https://docs.google.com/spreadsheets/d/1x-3Gzz8N1FMAonPvr5fjgSGiQlA-fobvylyuczHZ0X0/edit?usp=sharing)

************Advanced Version: ***************
Implementation: 
Code: https://colab.research.google.com/drive/1eMlJFjIB9WFr59GZjXgDKlGTHLQio964?usp=sharing 
![image](https://user-images.githubusercontent.com/37115711/228238130-ebd50c20-76a3-410c-a36f-e0f0189f0c50.png)

Resources: https://drive.google.com/drive/folders/1trNbzPiRSf8WV0L1QpFgHVMMbIY0UJbz?usp=sharing 


Testing: NOTE THAT ALL PICTURES ARE SELECTED RANDOMLY 
Training with 100 pictures, testing with 50 pictures: 
Execution time: 50 seconds

Training with 300 pictures, testing with 50 pictures(these are always the  same pictures which are already assessed by Dr.Armia) 
Execution time: 1 min 33seconds

Training with 488 Images and testing with 50 Images 
Execution time: 3minutes 57 seconds
Results: https://docs.google.com/spreadsheets/d/1x-3Gzz8N1FMAonPvr5fjgSGiQlA-fobvylyuczHZ0X0/edit?usp=sharing
![image](https://user-images.githubusercontent.com/37115711/228238007-46c5974b-ebce-4364-bf23-92273f099cc7.png)

3. SEated assessment based on video frames: 

Code for this solution: 
https://colab.research.google.com/drive/1UsWiGpAVA_NO7Xxv7He3AuHUx609ZsU9?usp=sharing 

We got Videos from: https://www.istockphoto.com/ 

Converted videos to mp4 format and adjusted resolution to have better results. 

Corrected code to take into account angle from where we are taking the videos. 

Tested the code with 5 videos of different durations, angles and visibility levels. 

For speed processing and robust processing video frames should exceed 20MB.

After Running the code You will the videos (original, converted, and results included) in this Drive Link: https://drive.google.com/drive/folders/1QEQaWY_Ii8Uw025xcYkmm48XfLOhY2BR?usp=sharing 






I ADDED COMMENTS AS MUCH AS POSSIBLE TO MAKE THE CODE CLEARER...
