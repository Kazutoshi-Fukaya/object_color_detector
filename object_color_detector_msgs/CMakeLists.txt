cmake_minimum_required(VERSION 3.0.2)
project(object_color_detector_msgs)

find_package(catkin REQUIRED COMPONENTS
    roscpp
    rospy
    std_msgs
    message_generation
)

add_message_files(
    FILES
    ObjectColorPosition.msg
    ObjectColorPositions.msg
)

generate_messages(
    DEPENDENCIES
    std_msgs
)

catkin_package(
    CATKIN_DEPENDS roscpp rospy std_msgs message_runtime
)
