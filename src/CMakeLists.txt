# Build the library.
add_library(rapidjson_ext
    JSON_Document.cpp
    JSON_Value.cpp
    JSON_Values.cpp
    )
target_link_libraries(rapidjson_ext ${LIBS})

# Installation rules.
install(TARGETS rapidjson_ext DESTINATION lib)
install(FILES
    JSON_Document.hpp
    JSON_Value.hpp
    JSON_Values.hpp
    DESTINATION include/rapidjson)
