set( HEADER_LIST 
  "${Easyloggingpp_SOURCE_DIR}/include/easyloggingpp/easylogging++.h"
)

set( SOURCES_LIST 
  "${Easyloggingpp_SOURCE_DIR}/src/easylogging++.cc"
)

add_library(easyloggingpp ${SOURCES_LIST} ${HEADER_LIST})
target_include_directories(easyloggingpp PUBLIC ../include)
target_compile_features(easyloggingpp PRIVATE cxx_std_17)
