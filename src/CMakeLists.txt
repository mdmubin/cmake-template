project(template_project)

# add any necessary include directories for you library here.
include_directories(
    include 
    ${CMAKE_SOURCE_DIR}/external/include
)

# source files
set(
    project_source_files
    # source file names go here
    example.cpp
)

# NOTE 
# if you are building an executable comment out library portion, and vice versa

# IF BUILDING LIBRARY ----------------------------------------------------------

# compile your source files
add_library(${PROJECT_NAME} ${project_source_files})

# export include for any builds using this library
target_include_directories(
    ${PROJECT_NAME}
    PUBLIC $<BUILD_INTERFACE:${PROJECT_SOURCE_DIR}/include>
)


# IF BUILDING APPLICATION ------------------------------------------------------

# set external library files directory
link_directories(${CMAKE_SOURCE_DIR}/external/libs)

# compile your source files
add_executable(${PROJECT_NAME} ${project_source_files})

# link any library required by the project
target_link_libraries(
    ${PROJECT_NAME}
    PRIVATE my_external_library
)
