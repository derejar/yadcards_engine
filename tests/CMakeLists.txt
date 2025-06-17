FetchContent_Declare(
    googletest
    GIT_REPOSITORY https://github.com/google/googletest.git
    GIT_TAG v1.15.x
    GIT_SHALLOW ON
    EXCLUDE_FROM_ALL
    SYSTEM
)
FetchContent_MakeAvailable(googletest)

add_executable(hellotest hellotest.cpp)
target_link_libraries(hellotest GTest::gtest_main)

include(GoogleTest)
gtest_discover_tests(hellotest EXTRA_ARGS --gtest_color=yes)


