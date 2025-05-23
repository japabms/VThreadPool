cmake_minimum_required(VERSION 3.10)
project(VThreadPool)

set(CMAKE_C_STANDARD 11)

set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/Build)
set(CMAKE_LIBRARY_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/Build)
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/Binaries)

<<<<<<< HEAD
add_library(vstring_static SHARED vthread_pool.c)
target_compile_options(vstring_static PRIVATE -g)
set_target_properties(vstring_static PROPERTIES OUTPUT_NAME "vthread-pool")

add_library(vstring_shared STATIC vthread_pool.c)
=======
add_library(vthread_pool_static SHARED vthread_pool.c)
target_compile_options(vstring_static PRIVATE -g)
set_target_properties(vstring_static PROPERTIES OUTPUT_NAME "vthread-pool")

add_library(vthread_pool_shared STATIC vthread_pool.c)
>>>>>>> d8aa25f (Initial commit.)
target_compile_options(vstring_shared PRIVATE -g)
set_target_properties(vstring_shared PROPERTIES OUTPUT_NAME "vthread-pool")

# add_executable(vstring_test Test.c)
# target_compile_options(vstring_test PRIVATE -g)
# set_target_properties(vstring_test PROPERTIES OUTPUT_NAME "test")
# target_link_libraries(vstring_test PRIVATE vstring_static)
