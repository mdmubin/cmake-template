project(template_project)


include_directories(include)

# source file names go here
set(
    project_source_files
    example.cpp
)

# IF BUILDING LIBRARY ----------------------------------------------------------

# compile your source files
add_library(${PROJECT_NAME} ${project_source_files})

# export include for any builds using this library
target_include_directories(
    ${PROJECT_NAME}
    PUBLIC $<BUILD_INTERFACE:${PROJECT_SOURCE_DIR}/include>
)
