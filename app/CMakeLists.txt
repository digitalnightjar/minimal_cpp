include(CTest)
enable_testing()

set(APP_INCLUDE_DIR "${CMAKE_CURRENT_SOURCE_DIR}/include")
include_directories(APP_INCLUDE_DIR)

add_executable(${PROJECT_NAME} src/main.cpp)
target_include_directories(${PROJECT_NAME} PRIVATE ${APP_INCLUDE_DIR})

# Link Libs
##===Add Here ===##


# CPack Installation Info
set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)