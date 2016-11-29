cmake_minimum_required(VERSION 3.0.0)
project(main_test VERSION 0.0.0)

include_directories(include)

# Add questions as a library items in here.
add_library(question1 STATIC src/Question1_1.cpp)

# Main execution is here
add_executable(main_test src/main.cpp)
target_link_libraries(main_test question1)

