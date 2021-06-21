# dual_ur5


  This is the Gazebo simulation configuration file of the ur5 dual-arm robot.
  
  Create two packages respectively, dual_ur_description and dual_ur_gazebo, the former stores the ur5 dual-arm model files, and the latter stores the related files of Gazebo.
Put all the files in the official ur_description function package in dual_ur_description, and create two new files dual_ur5_robot.urdf.xacro and dual_ur5_joint_limited_robot.urdf.xacro in the urdf file. The former represents the ur5 dual-arm model with unlimited joint motion. The former increases the joint restriction on the basis of the former. In addition, you need to   create a dual_ur5_upload.launch file in the launch folder to upload the xacro file of the dual-arm ur5 model to the parameter server.

  Also copy the official ur_gazebo file, create a new arm_controller_dual_ur.yaml file in the controller folder, which is used to load the controller parameters in Gazebo, create a new creation in the launch file and dual_ur5.launch to start the dual-arm ur5 simulation platform. 
