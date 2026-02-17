file(GLOB_RECURSE JOLT_SOURCES
    Jolt/*.cpp
)

add_library(Jolt STATIC ${JOLT_SOURCES})

# Mark Jolt include as SYSTEM to suppress warnings
target_include_directories(Jolt SYSTEM
    PUBLIC
        ${CMAKE_CURRENT_SOURCE_DIR}
)