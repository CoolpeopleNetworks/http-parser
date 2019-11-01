cmake_minimum_required(VERSION 3.0)
project(http_parser)

add_library(http_parser http_parser.c http_parser.h)

set_target_properties(http_parser PROPERTIES PUBLIC_HEADER "http_parser.h")

install(TARGETS http_parser
        PUBLIC_HEADER DESTINATION include
        LIBRARY DESTINATION lib
        )
