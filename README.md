# adversarial_image_classification

### Part 1
Introduce an alteration to the images that is imperceptible to the naked eye, but which renders its surveillance system inoperative.
The src/model.py script downloads a replica of the model which parses the images on the rogue system, saves it in the assets folder and runs a classification test.
In the assets folder you can find a test image. Crashing the model on that image is enough to conclude this part. Ideally, none of the RGB channel values of each pixel should be modified by more than one unit. modified by more than one unit. That is to say, if any pixel in the original image has values (120, 90, 90, 90, 90, 90, 120, 90, 90, 90, 90) original image has values (120, 90, 135), its value in the modified version of the image could be (121, 89, 136). could be (121, 89, 136).

### Part 2

Develop an image classification system that is as accurate as possible. In addition, the system should be resistant to attacks such as the one detailed in part 1 of the mission.
The goal is to train a system that can output as accurate a classification as possible within the taxonomy of the dataset.
In the src/dataset.py script you will find several ways to get the dataset.
