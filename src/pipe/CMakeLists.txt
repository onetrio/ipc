set(HEADERS pipe_sample.h)
set(SOURCES pipe_sample.c)

add_executable(pipe_pager pipe_pager.c)

add_library(pipe_sample STATIC 
            ${SOURCES} 
            ${HEADERS})

target_include_directories(pipe_sample PUBLIC .)