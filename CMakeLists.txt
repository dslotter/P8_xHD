cmake_minimum_required (VERSION 3.5)

project (xHDServer)

LINK_DIRECTORIES(/usr/local/lib /usr/lib/x86_64-linux-gnu)

SET(OTHER_LIBRARIES ${OTHER_LIBRARIES} -lserialport)

add_executable (xHDServer main.cpp)

target_link_libraries(xHDServer ${OTHER_LIBRARIES})
