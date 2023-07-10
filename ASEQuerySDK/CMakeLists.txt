# All Seeing Eye Query
add_library(ASEQuery STATIC IMPORTED GLOBAL
    ASEQuerySDK.h
    ASEQuerySDK.lib
)
target_include_directories(ASEQuery INTERFACE .)
set_target_properties(ASEQuery PROPERTIES IMPORTED_LOCATION ${CMAKE_CURRENT_SOURCE_DIR}/ASEQuerySDK.lib)
