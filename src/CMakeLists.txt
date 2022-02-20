add_subdirectory(main/c)

macro(add_seasocks_executable _name)
    add_executable(${_name} ${ARGN})
    target_link_libraries(${_name} PRIVATE seasocks)
endmacro()