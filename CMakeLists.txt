cmake_minimum_required (VERSION 2.8)
set( APPNAME tests )
project( ${APPNAME} )
add_definitions( "-Wall -g" )
include_directories( ./src )
AUX_SOURCE_DIRECTORY( ./src DIR_SRCS)
AUX_SOURCE_DIRECTORY( ./src/tests DIR_SRCS)
ADD_EXECUTABLE( ${APPNAME} ${DIR_SRCS} )
