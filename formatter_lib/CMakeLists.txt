cmake_minimum_required(VERSION 3.4)//задаем минимальную версию 
project(formatter) //задаем проект 
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
add_library(formatter_lib1 STATIC /formatter.cpp)//добавляем библиотеку 
add_executable(formatter /formatter.cpp)// компилирует исполняемый файл с заданным именем из списка исходников
target_link_libraries(formatter formatter_lib1) // компонует библиотеку или исполняемый файл с другими предоставляемыми библиотеками
