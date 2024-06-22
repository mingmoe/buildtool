
# quick js is a must
add_subdirectory("quickjs")

add_library(quickjspp INTERFACE)
target_link_libraries(quickjspp INTERFACE quickjs)
target_compile_features(quickjspp INTERFACE cxx_std_17)
set_target_properties(quickjspp PROPERTIES PUBLIC_HEADER quickjspp.hpp)

