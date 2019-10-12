cmake_minimum_required(VERSION 3.15)
project(enPAC)

set(CMAKE_CXX_STANDARD 14)
set(LINK_DIR /usr/local/lib)
link_directories(${LINK_DIR})
link_libraries(tcmalloc)
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -pthread")

include_directories(.)

add_executable(enPAC
        Data_Structures.cpp
        Data_Structures.h
        Lexer.cpp
        Lexer.h
        main.cpp
        Petri_Net.cpp
        Petri_Net.h
        product.cpp
        product.h
        RG.cpp
        RG.h
        SBA.cpp
        SBA.h
        Syntax_Tree.cpp
        Syntax_Tree.h
        TBA.cpp
        TBA.h
        TGBA.cpp
        TGBA.h
        tinystr.cpp
        tinystr.h
        tinyxml.cpp
        tinyxml.h
        tinyxmlerror.cpp
        tinyxmlparser.cpp
        xml2ltl.cpp
        xml2ltl.h)
