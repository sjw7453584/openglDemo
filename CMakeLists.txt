cmake_minimum_required(VERSION 2.8)
option(DEBUG_MODE "Debug or release?" ON)

if(DEBUG_MODE)
  set(CMAKE_BUILD_TYPE DEBUG)
else(DEBUG_MODE)
  set(CMAKE_BUILD_TYPE RELEASE)
endif(DEBUG_MODE)

set(CMAKE_CXX_FLAGS_DEBUG ${CMAKE_CXX_FLAGS} "-O0 -g")


project (openGlDemo)

add_subdirectory(polys)
# set(APP_NAME openGlDemo)
# add the executable
# set(SRCS
#   openGlDemoMain.cpp)
# add_executable(${APP_NAME}
#   ${SRCS}
# )

# target_link_libraries(${APP_NAME}
#   glut
#   GLU
#   GL
# )

# set(APP_BIN_DIR "${CMAKE_BINARY_DIR}/bin/")

# set_target_properties(${APP_NAME} PROPERTIES
#      RUNTIME_OUTPUT_DIRECTORY  "${APP_BIN_DIR}")
