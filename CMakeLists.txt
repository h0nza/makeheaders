cmake_minimum_required (VERSION 3.25 )

project (makeheaders VERSION 1.8 LANGUAGES C)

add_executable(makeheaders src/makeheaders.c)

# src/translate.c

#install

#tests
add_subdirectory(tests)
