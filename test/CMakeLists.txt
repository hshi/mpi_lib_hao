set(test_exe mpitest)

file(GLOB test_srcs "*.cpp")

add_executable(${test_exe} ${test_srcs})

target_link_libraries(${test_exe} mpihao)

install(TARGETS ${test_exe}  DESTINATION test)
