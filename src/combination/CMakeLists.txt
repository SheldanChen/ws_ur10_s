cmake_minimum_required(VERSION 2.8.3)

project(combination)

find_package(catkin REQUIRED)

catkin_package()

find_package(roslaunch)


find_package(catkin REQUIRED COMPONENTS
  urdf
  controller_manager
  joint_state_controller
  robot_state_publisher
  joint_state_publisher_gui
)

foreach(dir config launch meshes urdf)
	install(DIRECTORY ${dir}/
		DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/${dir})
endforeach(dir)
