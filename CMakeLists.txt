cmake_minimum_required(VERSION 3.10)
project(rm_description)

## Find catkin macros and libraries
find_package(ament_cmake REQUIRED
        COMPONENTS
        )

###################################
## catkin specific configuration ##
###################################
# catkin_package(
#         CATKIN_DEPENDS
# )

#############
## Install ##
#############

# Mark resource files for installation
install(
        DIRECTORY meshes urdf
        DESTINATION share/${PROJECT_NAME}
)

# Mark other files for installation
install(
        DIRECTORY doc
        DESTINATION share/${PROJECT_NAME}
)
install(
    DIRECTORY launch
    DESTINATION share/${PROJECT_NAME}/
)

ament_package()
