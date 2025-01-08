cmake_minimum_required(VERSION 3.10)

project(LocalCodeAssistant)

add_executable(locode src/main.cpp)

add_subdirectory(./llama.cpp)

target_link_libraries(locode llama)