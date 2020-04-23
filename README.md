[image1]: imgs/Screenshot_1.jpg "Architecture"
[image2]: imgs/Screenshot_2.jpg "Architecture"

#### System Architecture Diagram

The following is a system architecture diagram showing the ROS nodes and topics used in the project. You can refer to the diagram throughout the project as needed.

![alt text][image1] 

#### Code Structure
Below is a brief overview of the repo structure, along with descriptions of the ROS nodes. 

(path_to_project_repo)/ros/src/tl_detector/
This package contains the traffic light detection node: tl_detector.py. This node takes in data from the /image_color, /current_pose, and /base_waypoints topics and publishes the locations to stop for red traffic lights to the /traffic_waypoint topic.

The /current_pose topic provides the vehicle's current position, and /base_waypoints provides a complete list of waypoints the car will be following.

You will build both a traffic light detection node and a traffic light classification node. Traffic light detection should take place within tl_detector.py, whereas traffic light classification should take place within ../tl_detector/light_classification_model/tl_classfier.py.

![alt text][image2] 
