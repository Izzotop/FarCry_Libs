if(CMAKE_SIZEOF_VOID_P EQUAL 8)
    set(divx_media_lib DivxMediaLib64.lib)
else()
    set(divx_media_lib DivxMediaLib32.lib)
endif()

add_library(DivxMedia STATIC IMPORTED GLOBAL)
set_target_properties(DivxMedia PROPERTIES
    IMPORTED_LOCATION "${CMAKE_CURRENT_SOURCE_DIR}/${divx_media_lib}"
)
