project(template_project)

# add any necessary include directories for you library here.
include_directories(
    include 
    ${CMAKE_SOURCE_DIR}/external/include
)

# source file names go here
set(
    project_source_files
    example.cpp
)

# IF BUILDING LIBRARY ----------------------------------------------------------

# # compile your source files
# add_library(${PROJECT_NAME} ${project_source_files})

# # export include for any builds using this library
# target_include_directories(
#     ${PROJECT_NAME}
#     PUBLIC $<BUILD_INTERFACE:${PROJECT_SOURCE_DIR}/include>
# )

# IF BUILDING APPLICATION ------------------------------------------------------

link_directories(${CMAKE_SOURCE_DIR}/external/libs)

# compile your source files
add_executable(${PROJECT_NAME} ${project_source_files})

# link any library required by the project here
target_link_libraries(
    ${PROJECT_NAME}
    PRIVATE my_external_library
)
