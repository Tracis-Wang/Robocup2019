# RoboCup TOPIC LIST

### Decision

**subscribe**

| Type                       | Topic Name                 | Note                                 |
| :------------------------- | :------------------------- | :----------------------------------- |
| stereo_process::Ball       | "vision/ball"              | Bearing Range use Camera, not cloud! |
| stereo_process::Marker     | "vision/marker"            | Bearing Range use Camera, not cloud! |
| stereo_process::obstacles  | "vision/obstacles"         | Bearing Range use Camera, not cloud! |
| yolo_ros::BoundingBox      | "detection/ball"           |                                      |
| arm_head_motion::head_pose | "arm_head_motion/head_deg" |                                      |
| decision::UdpSend          | "/gait/Odometry"           |                                      |

**advertise**

| Type                       | Topic Name                 | Note |
| -------------------------- | -------------------------- | ---- |
| arm_head_motion::head_pose | "decision/head_command"    |      |
| decision::UdpReceived      | "/decision/command_to_udp" |      |

## yolo_ros

**subscribe**

| Type                       | Topic Name                   | Note |
| -------------------------- | ---------------------------- | ---- |
| sensor_msgs::ImageConstPtr | "/zed/left/image_rect_color" |      |

**advertise**

| Type                    | Topic Name           | Note |
| ----------------------- | -------------------- | ---- |
| yolo_ros::BoundingBox   | "/detection/ball"    |      |
| yolo_ros::BoundingBoxes | "/detection/objects" |      |



## depth_request

**subscribe**

| Type                        | Topic Name                          | Note |
| --------------------------- | ----------------------------------- | ---- |
| sensor_msgs::PointCloud2Ptr | "/zed/point_cloud/cloud_registered" |      |
| yolo_ros::BoundingBox       | "/detection/ball"                   |      |
| yolo_ros::BoundingBoxes     | "/detection/objects"                |      |
| arm_head_motion::head_pose  | "/arm_head_motion/head_deg"         |      |

**advertise**

| Type                      | Topic Name          | Note |
| ------------------------- | ------------------- | ---- |
| stereo_process::Ball      | "/vision/ball"      |      |
| stereo_process::Landmarks | "/vision/landmarks" |      |
| stereo_process::Goalpost  | "/vision/goalpost"  |      |
| stereo_process::Opponents | "/vision/opponents" |      |



## Location



## GameController


## Gait

