



https://drive.google.com/file/d/1JD3_SyqOZ6aHcZo_R1VX7z20OCK5kNNr/view


Vehicles have proven to be one of the most useful tools in daily lives. License plates are
used to identify unique vehicles in the legal system. As camera technologies develop, it has
shown great potential for Automatic License-Plate Recognition (ALPR) to replace manual
plate-reading. As a result, public agencies such as the police are already making use of this
technology for a variety of tasks. [1]
We propose to make an end-to-end ALPR system that, when given images, records the
plate numbers that were shown in that image. We believe the trained model can be applied
to both authority and civil utilizations. Also, since ALPR involves reading numbers, localising
the ROI and individualising symbols, we believe it is a valid project to be done in machine
learning.


Reading plate-numbers automatically has been a popular research direction since vehicles
had been around. Apparently, there were efforts made to make the task of reading
plate-numbers automatically as early as the 1980s. [5] Since the new millennium, there has
been an increasing number of research using machine learning. As a result, China has been
utilizing automatic license plate recognition technologies on detecting vehicle numbers
since the late 2000s to catch people driving restricted vehicles on a weekday of the week. A
recent paper shows that with their end-to-end lightweight CNN, 95% accuracy can be
achieved on live videos with Chinese license plates.


All the datasets we will be using are provided from a website that is offering Automatic
Number-plate Recognition service. [7] The dataset includes a large amount of plate images
with the plate's number as their labels.
The first group of dataset contains a group of low resolution and quality images that only
contains license plates. [8] The dataset groups images into 8 different categories. Each
license plate in each group has more than one picture in different conditions. Also, there is
a spreadsheet csv containing image paths and plate numbers. All group names ending with
“02” have test/validation data corresponding to the same name group ending with “01”.
However, we need to split non-training data into test and validation based on our
train:validation:test ratio.
The second group of dataset contains car pictures taken from the street. [9] This is used to
train our model to spot the license plate from a street view picture. This dataset has all
picture’s plate labels in text files, which we need to extract together with the paths, and
create a spreadsheet csv with, in the same format as the previous dataset. [8] We would be
loading data by taking in these csv files.
