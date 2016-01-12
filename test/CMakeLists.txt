cmake_minimum_required(VERSION 2.8)

include_directories(${GTEST_INCLUDE_DIR})

add_executable(client_tests ../src/test_client.cc test_test_client.cc)

target_link_libraries(client_tests PUBLIC ${GTEST_LIBRARY} ${GTEST_MAIN_LIBRARY})