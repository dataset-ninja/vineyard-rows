The **Semantic Segmentation Vineyard Rows** dataset is the result of work in which the authors presented a new low-cost and accessible edge motion control system for autonomous navigation in vineyard rows. It uses the properties of semantic segmentation provides a proportional controller that controls the robot area along the entire row without touching the vine plants. Precision agriculture is a fast-growing field that aims at introducing affordable and effective automation into agricultural processes. The dataset includes 500 RGB - images with the relative single-channel binary masks.

## Dataset creation methodology

The authors research group aims at developing an affordable self-driving system for vineyard parcels. Given a global path made of georeferenced waypoints, they exploit a dual local planner to overcome the lack of accuracy of the GPS based localization filter inside the vine rows. Eventually, all the algorithms have been developed ROScompatible, in order to make easier the communication among them and to be easily deployed on developing platform; the Jackal Unmanned Ground Vehicle (UGV) by Clearpath Robotics3, that is fully supported by the Robot Operating System (ROS).

<img src="https://github.com/dataset-ninja/vineyard-rows/assets/120389559/726fde89-f432-477a-9c34-14a9f58cd946" alt="image" width="600" height="600">

<span style="font-size: smaller; font-style: italic;">The Jackal Unmanned Ground Vehicle in Grugliasco, Turin, North of Italy.</span>

The authors propose a control algorithm to perform real-time autonomous navigation along the vineyard rows that leverages the latest advancement on edge AI to obtain a continuous and reliable control with a low-range hardware setup. The devised system exploits the joint information of RGB and depth inputs, cutting costs of expensive sensors and overcoming issues experienced by solutions based on GPS devices.

## Dataset description

In order to create a dataset for training and testing the deep neural network, the authors carry out field surveys in two distinct agricultural areas in the North of Italy: Grugliasco near Turin in Piedmont region and Valle San Giorgio di Baone in the Province of Padua in the Veneto region. The data is collected at different times of the day, with diverse weather conditions, and they present a variety of terrain types and wine qualities. To have different perspectives inside the vineyard rows, the authors acquire several videos with only three fixed orientations: one pointing the camera at the center of the vineyard row and the other two pointing to the left and right sides, respectively. For training and testing, the authors select one frame every 25 in order to work with quite different scenarios. Finally, to generate the masks for the supervised training, they exploit the collected images by first manually annotating them, and successively refining the obtained binary masks using a Gaussian mixture model in order to train and evaluate the network with more accurate masks.

<img src="https://github.com/dataset-ninja/vineyard-rows/assets/120389559/5e2ffa99-ae12-4533-b097-33053f570176" alt="image" width="800">

<span style="font-size: smaller; font-style: italic;">In a, b and c are shown three instances of the dataset, one for each video orientation. a is an example left samples, b center, and c right. d, e and f are the corresponding binary masks for the supervised training. Dataset samples have been collected with different weather conditions and at different times of the day.</span>
