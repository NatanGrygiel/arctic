cmake_minimum_required(VERSION 3.28)
project(arctic)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTORCC ON)
set(CMAKE_AUTOUIC ON)


find_package(Qt6 COMPONENTS
        Core
        Gui
        Widgets
        REQUIRED)

add_executable(arctic main.cpp)
target_link_libraries(arctic
        Qt::Core
        Qt::Gui
        Qt::Widgets
)

