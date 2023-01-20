cmake_minimum_required(VERSION 3.15)
project(openssl_project C)

find_package(OpenSSL)

add_executable(${PROJECT_NAME} src/main.c)

# Use the global target
target_link_libraries(${PROJECT_NAME} openssl::openssl)
