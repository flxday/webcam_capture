#indicate minimum version
CMAKE_MINIMUM_REQUIRED(VERSION 2.6)

#project name
PROJECT(webcam_capture)

#find required packages (look for the package, usually at /usr/share/cmake-2.8/Modules/ or /usr/share/)
FIND_PACKAGE(OpenCV REQUIRED)

#set header directories
INCLUDE_DIRECTORIES(${OpenCV_INCLUDE_DIR})

#Create an executable
ADD_EXECUTABLE(webcam_capture src/webcam_capture.cpp)

#Link with libraries
TARGET_LINK_LIBRARIES(webcam_capture ${OpenCV_LIBS})

# Setting this prefix will be used by INSTALL commands in next CMakeLists
SET(CMAKE_INSTALL_PREFIX /usr/local)

#install
INSTALL(TARGETS webcam_capture RUNTIME DESTINATION bin)