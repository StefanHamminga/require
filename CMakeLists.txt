cmake_minimum_required (VERSION 3.8)
project (require VERSION 0.0.0)

add_library(
    ${PROJECT_NAME}
    INTERFACE
)

install(FILES
    std/c++11
    std/c++14
    std/c++17
    std/c++2a
    std/gnu++11
    std/gnu++14
    std/gnu++17
    std/gnu++2a
    DESTINATION
    include/${PROJECT_NAME}/std
)

# install(FILES
#     feature/.....
#     DESTINATION
#     include/${PROJECT_NAME}/feature
# )
