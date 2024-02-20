#[[https://github.com/mbed-ce/mbed-os/wiki/MbedOS-configuration#libraries-in-your-application]]

#[[ Set name of library in lowcase]]
set(INTERNAL_LIBRARY_NAME "mbed-http")

#[[ Here fill all .cpp files]]
add_library(${INTERNAL_LIBRARY_NAME} STATIC http_parser/http_parser.c)

#[[ Include .h files]]
target_include_directories(${INTERNAL_LIBRARY_NAME} INTERFACE ./http_parser/ ./source/)

#[[Link library to mbed-core-flags but if the library needs to use RTOS
 features, then have to be add also mbed-rtos-flags]]
target_link_libraries(${INTERNAL_LIBRARY_NAME} PUBLIC mbed-core-flags)