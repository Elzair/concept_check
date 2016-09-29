cmake_minimum_required(VERSION 3.3)

project(boost_concept_check)

add_library(boost_concept_check INTERFACE)

target_include_directories(boost_concept_check BEFORE INTERFACE ${CMAKE_CURRENT_SOURCE_DIR}/include)

install(TARGETS boost_concept_check DESTINATION lib)
install(DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/include/boost DESTINATION include)
