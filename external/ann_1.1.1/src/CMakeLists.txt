set(ANN_CPP
    ANN.cpp
    brute.cpp
    kd_tree.cpp
    kd_util.cpp
    kd_split.cpp
    kd_dump.cpp
    kd_search.cpp
    kd_pr_search.cpp
    kd_fix_rad_search.cpp
    bd_tree.cpp
    bd_search.cpp
    bd_pr_search.cpp
    bd_fix_rad_search.cpp
    perf.cpp
    )


add_library(${ANN_TARGET_LIB} ${ANN_CPP})

install(TARGETS ${ANN_TARGET_LIB}
    LIBRARY DESTINATION lib
    ARCHIVE DESTINATION lib
    )
