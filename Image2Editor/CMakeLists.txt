file(GLOB_RECURSE SOURCE Source/*.h Source/*.cpp)

add_executable("Image2Editor" "${SOURCE}")

set_target_properties("Image2Editor" PROPERTIES LINKER_LANGUAGE CXX)

target_link_libraries("Image2Editor" PUBLIC "Image2ExcelC")

file(COPY Resources DESTINATION "${CMAKE_BINARY_DIR}/Image2Editor")