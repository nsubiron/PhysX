cmake_minimum_required(VERSION 3.10)

project(PhysXSDK C CXX)

set(PHYSX_ROOT_DIR "${PROJECT_SOURCE_DIR}/physx")
set(PX_OUTPUT_LIB_DIR "${PROJECT_SOURCE_DIR}/physx")
set(PX_OUTPUT_BIN_DIR "${PROJECT_SOURCE_DIR}/physx")

set(ENV{PM_CMakeModules_PATH} "${PROJECT_SOURCE_DIR}/externals/cmakemodules")
set(ENV{PM_PATHS} "${PROJECT_SOURCE_DIR}/externals/opengl-linux;${PROJECT_SOURCE_DIR}/externals/targa;${PROJECT_SOURCE_DIR}/externals/cg-linux;${PROJECT_SOURCE_DIR}/externals/glew-linux")
set(ENV{PM_PxShared_PATH} "${PROJECT_SOURCE_DIR}/pxshared")

add_subdirectory("physx/compiler/public")
