#
#  CMakeLists.txt
#  minizip
#
#  Created by Dmitrii Torkhov <dmitriitorkhov@gmail.com> on 07.02.2022.
#  Copyright © 2022 Dmitrii Torkhov. All rights reserved.
#

set(SRC
        minizip/ioapi.cpp
        minizip/unzip.cpp
        minizip/ioapi_mem.cpp)

add_library(minizip STATIC ${SRC})

#

target_include_directories(minizip
        PUBLIC $<BUILD_INTERFACE:${CMAKE_CURRENT_LIST_DIR}/../include>
        PUBLIC $<BUILD_INTERFACE:${CMAKE_CURRENT_LIST_DIR}/../include/minizip>
        PUBLIC $<BUILD_INTERFACE:${CMAKE_CURRENT_LIST_DIR}/minizip>)

set_target_properties(minizip PROPERTIES CXX_STANDARD 17 CXX_STANDARD_REQUIRED YES CXX_EXTENSIONS NO)