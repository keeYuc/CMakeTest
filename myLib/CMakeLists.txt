aux_source_directory(./ all)
set(LIBRARY_OUTPUT_PATH ../lib)
add_library(myLib STATIC ${all})