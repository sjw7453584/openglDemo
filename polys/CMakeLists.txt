set(APP_NAME polys)
# add the executable
set(SRCS
  polys.c)
add_executable(${APP_NAME}
  ${SRCS}
)

target_link_libraries(${APP_NAME}
  glut
  GLU
)

set(APP_BIN_DIR "${CMAKE_BINARY_DIR}/bin/")

set_target_properties(${APP_NAME} PROPERTIES
     RUNTIME_OUTPUT_DIRECTORY  "${APP_BIN_DIR}")
