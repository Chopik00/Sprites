set(CMAKE_VERSION 3.20)
cmake_minimum_required(VERSION ${CMAKE_VERSION})

project("Hello OpenGL" VERSION 0.1.0)

set(SOURCES
  "src/main.cpp"
)

add_executable(app ${SOURCES})

set_target_properties(app PROPERTIES
  RUNTIME_OUTPUT_NAME "Sprites_v${PROJECT_VERSION}"
  RUNTIME_OUTPUT_DIRECTORY "${CMAKE_CURRENT_LIST_DIR}/bin"
)