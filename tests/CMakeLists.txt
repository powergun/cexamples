
add_tinytest_executable(loadTestData _testdata/test_load.c)
target_link_libraries(loadTestData testdata)
add_test(NAME "testdata::loaderTest" COMMAND loadTestData)

add_subdirectory(IO)
add_subdirectory(memory)
add_subdirectory(algorithms)
add_subdirectory(arithmetics)

add_subdirectory(parallel/pthread)
add_subdirectory(parallel/posix_fork)
add_subdirectory(string)
add_subdirectory(casting)