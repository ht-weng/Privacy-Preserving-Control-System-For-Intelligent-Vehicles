cmake_minimum_required(VERSION 3.12)

project(MAIN VERSION 1.0 LANGUAGES CXX)

# add_executable(pid pid.cpp)

# add_executable(pid-controller pid-controller.cpp)

# add_executable(bergman bergman.cpp)

add_executable(pid-serialize-test pid-serialize-test.cpp)

find_package(SEAL 3.6 REQUIRED)

find_package(Boost REQUIRED)

# Link Microsoft SEAL
# target_link_libraries(pid SEAL::seal)

# target_link_libraries(pid-controller SEAL::seal)

# target_link_libraries(bergman SEAL::seal)

target_link_libraries(pid-serialize-test SEAL::seal)

