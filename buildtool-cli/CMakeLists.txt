# CMakeList.txt: buildtool 的 CMake 项目，在此处包括源代码并定义
# 项目特定的逻辑。
#

# 将源代码添加到此项目的可执行文件。
add_executable (buildtool_cli "buildtool.cpp" "buildtool.h")

set_property(TARGET buildtool_cli PROPERTY CXX_STANDARD 23)

target_link_libraries(buildtool_cli PRIVATE buildtool_lib)

# TODO: 如有需要，请添加测试并安装目标。
