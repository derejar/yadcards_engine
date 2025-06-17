add_executable(${PROJECT_NAME} main.cpp)

add_subdirectory(StateMachine)

target_link_libraries(${PROJECT_NAME}
    PUBLIC
        StateMachine
)
