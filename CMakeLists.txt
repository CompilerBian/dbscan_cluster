cmake_minimum_required(VERSION 2.8.3)
project(dbscan_cluster)


find_package(catkin REQUIRED COMPONENTS
  geometry_msgs
  roscpp
  rospy
  sensor_msgs
  std_msgs
  message_generation
  pcl_conversions
  pcl_ros
)


generate_messages(
  DEPENDENCIES
  std_msgs
)


catkin_package()


include_directories(
  ${catkin_INCLUDE_DIRS}
)
