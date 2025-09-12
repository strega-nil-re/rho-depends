cmake_minimum_required(VERSION 4.0)
include(cmake/rho-boot.cmake)

set(RHO_CXX_STANDARD 23)
project(depends)
rho_add_executable(depends)

rho_find_package(mu REQUIRED)
target_link_libraries(depends PRIVATE mu::mu)
