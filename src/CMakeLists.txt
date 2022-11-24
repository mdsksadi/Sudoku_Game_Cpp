# add source and header files when compiling the given target.
# although it is not necessary to add header files, we also do that for easing the management of IDE.
target_sources(${CURRENT_EXE_NAME}
    PUBLIC
        ${CMAKE_CURRENT_LIST_DIR}/altproj.cpp
        ${CMAKE_CURRENT_LIST_DIR}/game.cpp
        ${CMAKE_CURRENT_LIST_DIR}/solver.cpp
        ${CMAKE_CURRENT_LIST_DIR}/tests.cpp
        ${CMAKE_CURRENT_LIST_DIR}/debug.cpp
)

# add current directory to the compiler included directories when compiling the given target.
target_include_directories(${CURRENT_EXE_NAME} PUBLIC "${CMAKE_CURRENT_LIST_DIR}")

