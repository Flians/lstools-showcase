add_executable(abc2 abc.cpp)
target_link_libraries(abc2 alice libabc-pic)

add_alice_python_module(abc2 abc.cpp)
target_link_libraries(abc2_python PRIVATE libabc-pic)

add_alice_c_library(abc2 abc.cpp)
target_link_libraries(abc2_c PRIVATE libabc-pic)
