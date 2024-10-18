# HTTP/S library for MbedCE

This library is used to make HTTP and HTTPS calls from Mbed OS applications.

## How to start
1. Create a new project according to [MbedCE instructions](https://github.com/mbed-ce/mbed-os/wiki)
2. Add this as submodule to your project via `git submodule add --depth 1 https://github.com/mbed-ce-libraries-examples/mbed-http mbed-http`
3. The top level `CMakeList.txt` (in root of your project) should be modified according to [this wiki page](https://github.com/mbed-ce/mbed-os/wiki/MbedOS-configuration#libraries-in-your-application)
    Don't forget link also  `mbed-netsocket`, then the link part in top lvl CMake should look like `target_link_libraries(${CMAKE_PROJECT_NAME}  mbed-os mbed-netsocket)`
4. Copy & Paste one example from Test folder into project folder.
5. Build the project


## Example code
Examples are in [TEST folder](https://github.com/mbed-ce-libraries-examples/mbed-http/tree/master/TESTS).

## Description
You can look to [README_mbed-http.md](https://github.com/mbed-ce-libraries-examples/mbed-http/blob/master/README_mbed-http.md)

### Status:
This library was tested (02/2024) with Nucleo-F767ZI, VS-Code under Win11, GCC 12.3 and MbedCE library

Fork of https://os.mbed.com/teams/sandbox/code/mbed-http/
