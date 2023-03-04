cmake_minimum_required(VERSION 3.21)

project(BourseDePoche VERSION 0.1 LANGUAGES CXX)

find_package(QT NAMES Qt6 Qt5 REQUIRED COMPONENTS Core Quick)

set(PROJECT_SOURCES
        main.cpp
        qml.qrc
)

add_executable(BourseDePoche
    ${PROJECT_SOURCES}
)