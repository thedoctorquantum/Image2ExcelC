file(GLOB_RECURSE SOURCE Source/*.c Source/*.cpp)
file(GLOB_RECURSE INCLUDE Source/*.h Source/*.hpp)

add_library("Image2Excel" STATIC "${SOURCE}" "${INCLUDE}")

set_target_properties("Image2Excel" PROPERTIES LINKER_LANGUAGE CXX)

target_include_directories("Quanta" PUBLIC 
    "${CMAKE_CURRENT_SOURCE_DIR}/Source"
)

#target_link_libraries("Quanta" "")