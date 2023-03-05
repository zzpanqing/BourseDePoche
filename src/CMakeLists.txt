cmake_minimum_required(VERSION 3.21)

project(BourseDePoche VERSION 0.1 LANGUAGES CXX)

find_package(Qt6 6.2 REQUIRED COMPONENTS Gui Core Quick)
find_package(Qt6Gui REQUIRED)

set(PROJECT_SOURCES
        main.cpp
        qml.qrc
)

add_executable(BourseDePoche
    ${PROJECT_SOURCES}
)

target_link_libraries(${PROJECT_NAME} Qt6::Gui Qt6::Quick)