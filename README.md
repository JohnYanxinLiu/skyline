# skyline
A Robot Arm to stack Jenga blocks


To Get Started with the Simulator:
`git clone git@github.com:JohnYanxinLiu/skyline.git`
`cd skyline/skyline_ws`
`catkin build`

launch the simulator with:
`source /opt/ros/noetic/setup.bash`
`roscore`
In another terminal, run
`source /opt/ros/noetic/setup.bash`
`source skyline/skyline_ws/devel/setup.bash`
`roslaunch simulator_pkg skyline.launch`

Notes:
- Followed [this tutorial] {https://www.youtube.com/watch?v=p9g-5OLhynA&list=PLeEzO_sX5H6TBD6EMGgV-qdhzxPY19m12} to create
- Used [sw to urdf] {http://wiki.ros.org/sw_urdf_exporter} plugin on Solidworks 2022 to export model
- Found issue while launching where `position_controllers/JointTrajectoryController` doesn't start. Followed [this page] {https://answers.ros.org/question/354898/controller-type-position_controllersjointtrajectorycontroller-does-not-exist/} and ran `sudo apt-get install ros-noetic-joint-trajectory-controller` to solve the issue.
- Also followed [this page] {https://answers.ros.org/question/363603/gazebo-controller-not-started/} to run `sudo apt-get install ros-noetic-gazebo-ros-control joint-state-publisher` `sudo apt-get install ros-kinetic-controller-manager`
