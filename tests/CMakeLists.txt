cmake_minimum_required(VERSION 3.25)

project(abc VERSION 1.0 LANGUAGES C)

add_executable(abc abc.c a.c b.c c.c)


add_custom_command(OUTPUT abc.h
COMMAND $<TARGET_FILE:makeheaders> -h a.c b.c c.c
MAIN_DEPENDENCY abc.h
BYPRODUCTS a.h
)

#add_custom_target()
