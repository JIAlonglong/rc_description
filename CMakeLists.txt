cmake_minimum_required(VERSION 3.0.2)
project(rc_description)

## Find catkin macros and libraries
find_package(catkin REQUIRED
        COMPONENTS
        )

###################################
## catkin specific configuration ##
###################################
catkin_package(
        CATKIN_DEPENDS
)

#############
## Install ##
#############

# Mark resource files for installation
install(
        DIRECTORY meshes urdf
        DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)

# Mark other files for installation
install(
        DIRECTORY doc
        DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)
