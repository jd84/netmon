include_directories ("${PROJECT_SOURCE_DIR}/src")

add_executable(netmon-example main.cpp)

target_link_libraries(netmon-example netmon)
