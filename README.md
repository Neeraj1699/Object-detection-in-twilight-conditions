# Object-detection-in-twilight-conditions
# AIM
To detect a high ratio of the objects such as cars, pedestrians, trucks, autorickshaws, motorcycles, etc present in the input database.
# METHODOLOGY
We created a custom dataset with autorickshaws that are available all over India.
We annotated the region of interest for each image in the test and train sets. This includes specifying the following parameters for each image :
Object class
X_center
Y_center
Normalised height and width of the bounding box
We were able to acquire 800 images. 
We made several changes to the configuration files(yolo-obj.cfg) of the source code for this purpose. Some of the key changes include: 
batch size
iteration steps
number of filters in each layer
Number of subdivisions
Max classes
Object data file
# INNOVATIVE ABOUT US
During testing with various datasets, we observed that YOLO v4 was not able to detect autorickshaws(commonly found vehicle on Indian roads) and confused it with trucks. 
Given the high accuracy rate and fast speed, incorporating this class would be a huge add-on to this algorithm. So we did quite a few modifications to the original program and added a separate class for autorickshaws

