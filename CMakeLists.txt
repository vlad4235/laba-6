cmake_minimum_required(VERSION 3.15)

# Название проекта
project(main 6.1)

# Устанавливаем стандарт C++
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED True)

# Добавляем файлы исходного кода
set(SOURCES
    main 6.1.cpp
    Figure.cpp
    Parallelogram.cpp
    Triangle.cpp
    Point.cpp
)

set(HEADERS
    Figure.h
    Parallelogram.h
    Triangle.h
    Point.h
)

# Создаем исполняемый файл из указанных исходников
add_executable(main 6.1 ${SOURCES} ${HEADERS})

# Добавляем включаемые каталоги
target_include_directories( main 6.1 PRIVATE .)
