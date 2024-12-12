cmake_minimum_required(VERSION 2.40.3)

set(PROJECT_NAME custom-learn)
set(SOURCE_DIR ${CMAKE_SOURCE_DIR}/src)
SET(HEADERS_DIR ${SOURCE_DIR}/private)

project(${PROJECT_NAME})

file(GLOB SOURCE_FILES "${SOURCE_DIR}/*.cpp")
file(GLOB HEADER_FILES "${HEADERS_DIR}/private")

add_executable(${PROJECT_NAME} ${SOURCE_FILES} ${HEADERS_FILES})