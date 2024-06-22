
add_library (buildtool_lib "buildtool.cpp" "buildtool.h")

set_property(TARGET buildtool_lib PROPERTY CXX_STANDARD 23)

target_link_libraries (buildtool_lib PRIVATE quickjspp)

