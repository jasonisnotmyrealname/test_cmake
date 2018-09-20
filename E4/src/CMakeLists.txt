#add include directory to the build,其中PROJECT_SOURCE_DIR指的是most recent project() command
include_directories(${PROJECT_SOURCE_DIR}/libhello)

set(APP_SRC main.c)
add_executable(hello ${APP_SRC})
target_link_libraries(hello libhello)
