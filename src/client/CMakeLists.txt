project(TiaraCE-Client)

###############################################################################
# Source Files
###############################################################################
set(src_files
"client.cpp"
)

###############################################################################
# Library Files
###############################################################################
set(lib_files
${SDL2_LIBRARIES}
)

###############################################################################
# Compiler
###############################################################################
add_executable(TiaraCE-Client ${src_files})

###############################################################################
# Linker
###############################################################################
target_link_libraries(TiaraCE-Client TiaraCE-Engine ${lib_files})
