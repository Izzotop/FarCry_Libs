add_library(Bink STATIC IMPORTED GLOBAL
    bink.h

#    dx7rad3d.cpp
#    dx8rad3d.cpp

    glrad3d.c
    RAD.H
    rad3d.h
    radbase.h
    radmem.h
)
target_include_directories(Bink INTERFACE .)
set_target_properties(Bink PROPERTIES IMPORTED_LOCATION ${CMAKE_CURRENT_SOURCE_DIR}/binkw32.lib)
