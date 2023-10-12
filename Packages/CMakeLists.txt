project(Packages)
add_library(${PROJECT_NAME} INTERFACE)
add_subdirectory(wxWidgets)


# Link the libraries to ${PROJECT_NAME}

target_link_libraries(${PROJECT_NAME} INTERFACE  wx::net wx::core wx::base)
