idf_component_register()

# include(ExternalProject)

add_library(MCP251XFD_lib "${CMAKE_CURRENT_SOURCE_DIR}/MCP251XFD.c")
target_include_directories(MCP251XFD_lib INTERFACE "${CMAKE_CURRENT_SOURCE_DIR}")
target_link_libraries(${COMPONENT_LIB} INTERFACE MCP251XFD_lib)