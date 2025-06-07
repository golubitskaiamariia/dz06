cmake_minimum_required(VERSION 3.8)
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

project(FormatterProject)

add_subdirectory(formatter_lib)
add_subdirectory(formatter_ex_lib)
add_subdirectory(solver_lib)

add_subdirectory(solver_application)
add_subdirectory(hello_world_application)

set(CPACK_PACKAGE_NAME "dz_lab06")
set(CPACK_PACKAGE_VERSION "1.0.0")
set(CPACK_DEBIAN_PACKAGE_MAINTAINER "Plisya")
set(CPACK_GENERATOR DEB RPM WIX DragNDrop TGZ ZIP)
include(CPack)
