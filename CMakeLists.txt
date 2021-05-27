project(travisexample)
cmake_minimum_required(VERSION 3.5)

# set_target_properties(${PROJECT_NAME}
#     PROPERTIES
#     # ARCHIVE_OUTPUT_DIRECTORY "/home/xy/cmake_practice/lib/"
#     # LIBRARY_OUTPUT_DIRECTORY "/home/xy/cmake_practice/lib/"
#     RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/bin/
# )
# set(
#     #   ARCHIVE_OUTPUT_DIRECTORY "/home/xy/cmake_practice/lib/"
#     #   LIBRARY_OUTPUT_DIRECTORY "/home/xy/cmake_practice/lib/"
#       RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/bin/
# )
set(EXECUTABLE_OUTPUT_PATH bin)

# include(conanbuildinfo.cmake)
# conan_basic_setup()

message(WARNING ${RUNTIME_OUTPUT_DIRECTORY})

add_executable(${PROJECT_NAME} src/main.cpp)
# target_link_libraries(${PROJECT_NAME} ${CONAN_LIBS}) # note the conan libs over here
