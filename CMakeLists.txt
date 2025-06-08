#--------------------------------- FILE INFO ----------------------------------#
# Filename           : CMakeLists.txt                                          #
#                                                                              #
# Top level CMakeLists.txt file                                                #
#                                                                              #
#------------------------------------------------------------------------------#
cmake_minimum_required(VERSION 4.0.2)
project(hello_world_lib LANGUAGES C)

include(FetchContent)

# \/ === ADD ALL GITHUB PROJECT DEPENDENCIES HERE === \/
#FetchContent_Declare(
#    #fetched_item_name_here
#    GIT_REPOSITORY https://github.com/Mouse-Unit-07/software-hello-world.git
#    GIT_TAG main
#)
#FetchContent_MakeAvailable(#fetched_item_name_here)

add_library(hello_world_lib STATIC)

# \/ === ADD SOURCE SUBDIRECTORIES HERE === \/
add_subdirectory(hello_world)

target_include_directories(hello_world_lib PUBLIC
    ${CMAKE_CURRENT_SOURCE_DIR}/hello_world
)

# \/ === LINK TO GITHUB DEPENDENCIES HERE === \/
#target_link_libraries(hello_world_lib PUBLIC
#    #library_name_here
#)