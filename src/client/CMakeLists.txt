set(target_name client)

include_directories(${Boost_INCLUDE_DIR})

add_executable(${target_name}
    Client.cpp
    main.cpp
    Stream.cpp
)

target_link_libraries(${target_name}
    ${Boost_LIBRARIES}
    ${OpenCV_LIBS}
)
