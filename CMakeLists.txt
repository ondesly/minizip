#
#  CMakeLists.txt
#  minizip
#
#  Created by Dmitrii Torkhov <dmitriitorkhov@gmail.com> on 07.02.2022.
#  Copyright © 2022 Dmitrii Torkhov. All rights reserved.
#

cmake_minimum_required(VERSION 3.14 FATAL_ERROR)

project(minizip
        VERSION 1.0.0
        LANGUAGES C CXX)

#########
# Build #
#########

add_subdirectory(src)