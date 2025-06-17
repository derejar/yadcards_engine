set(LIBRARY_NAME StateMachine)

add_library(${LIBRARY_NAME} STATIC)

target_sources(${LIBRARY_NAME}
    PRIVATE
        StateMachine.cpp
    PUBLIC
        StateMachine.h
)
