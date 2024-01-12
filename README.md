# skyline
A Robot Arm to stack Jenga blocks


Start:
git clone TODO
cd skyline/skyline_ws
catkin_make

launch the simulator with
roslaunch simulator_pkg skyline.launch

Notes:
- Followed [this tutorial] {https://www.youtube.com/watch?v=p9g-5OLhynA&list=PLeEzO_sX5H6TBD6EMGgV-qdhzxPY19m12} to create
- Used [sw to urdf] {http://wiki.ros.org/sw_urdf_exporter} plugin on Solidworks 2022 to export model
- Found issue while launching where `position_controllers/JointTrajectoryController` doesn't start. Followed [this page] {https://answers.ros.org/question/354898/controller-type-position_controllersjointtrajectorycontroller-does-not-exist/} and ran `sudo apt-get install ros-noetic-joint-trajectory-controller` to solve the issue.
- Also followed [this page] {https://answers.ros.org/question/363603/gazebo-controller-not-started/} to run `sudo apt-get install ros-noetic-gazebo-ros-control joint-state-publisher` `sudo apt-get install ros-kinetic-controller-manager`
