# this is for emacs file handling -*- mode: cmake; indent-tabs-mode: nil -*-

# -- BEGIN LICENSE BLOCK ----------------------------------------------
# -- END LICENSE BLOCK ------------------------------------------------

#----------------------------------------------------------------------
#
# \author  Andreas Hermann
# @date    2014-06-11
#
#----------------------------------------------------------------------

#------------- Example Program for the usage of gpu_voxels ------------
ICMAKER_SET("collisions" IDE_FOLDER ${EXAMPLES_IDE_FOLDER})

ICMAKER_ADD_HEADERS(
  )

ICMAKER_ADD_SOURCES(
  Collisions.cpp
  )

ICMAKER_ADD_CUDA_FILES(
  )

ICMAKER_LOCAL_CPPDEFINES(-DGPU_VOXELS_EXPORT_SYMBOLS -Wno-unknown-pragmas)
ICMAKER_GLOBAL_CPPDEFINES(-D_IC_BUILDER_GPU_VOXELS_EXAMPLES_COLLISION_)
ICMAKER_INCLUDE_DIRECTORIES(${GPU_VOXELS_INCLUDE_DIRS})

ICMAKER_INTERNAL_DEPENDENCIES(
  icl_core
  icl_core_config
  icl_core_logging
  gpu_voxels
  )

ICMAKER_EXTERNAL_DEPENDENCIES(
  CUDA
  )

ICMAKER_BUILD_PROGRAM()

#------------- Example Program for the usage of gpu_voxels ------------
ICMAKER_SET("maps" IDE_FOLDER ${EXAMPLES_IDE_FOLDER})

ICMAKER_ADD_HEADERS(
  )

ICMAKER_ADD_SOURCES(
  Maps.cpp
  )

ICMAKER_ADD_CUDA_FILES(
  )

ICMAKER_LOCAL_CPPDEFINES(-DGPU_VOXELS_EXPORT_SYMBOLS -Wno-unknown-pragmas)
ICMAKER_GLOBAL_CPPDEFINES(-D_IC_BUILDER_GPU_VOXELS_EXAMPLES_MAPS_)
ICMAKER_INCLUDE_DIRECTORIES(${GPU_VOXELS_INCLUDE_DIRS})

ICMAKER_INTERNAL_DEPENDENCIES(
  icl_core
  icl_core_config
  icl_core_logging
  gpu_voxels
  )

ICMAKER_EXTERNAL_DEPENDENCIES(
  CUDA
  )

ICMAKER_BUILD_PROGRAM()
#------------- Example Program for the usage of gpu_voxels ------------
ICMAKER_SET("shift_vs_transform" IDE_FOLDER ${EXAMPLES_IDE_FOLDER})

ICMAKER_ADD_HEADERS(
  )

ICMAKER_ADD_SOURCES(
  ShiftVsTransform.cpp
  )

ICMAKER_ADD_CUDA_FILES(
  )

ICMAKER_LOCAL_CPPDEFINES(-DGPU_VOXELS_EXPORT_SYMBOLS -Wno-unknown-pragmas)
ICMAKER_GLOBAL_CPPDEFINES(-D_IC_BUILDER_GPU_VOXELS_EXAMPLES_SHIFT_VS_TRANSFORM_)
ICMAKER_INCLUDE_DIRECTORIES(${GPU_VOXELS_INCLUDE_DIRS})

ICMAKER_INTERNAL_DEPENDENCIES(
  icl_core
  icl_core_config
  icl_core_logging
  gpu_voxels
  )

ICMAKER_EXTERNAL_DEPENDENCIES(
  CUDA
  PCL
  )

ICMAKER_BUILD_PROGRAM()

#------------- Example Program for the usage of height-maps ------------
ICMAKER_SET("heightmap_loader" IDE_FOLDER ${EXAMPLES_IDE_FOLDER})

ICMAKER_ADD_SOURCES(
  HeightmapLoader.cpp
  )

ICMAKER_ADD_CUDA_FILES(
  )

ICMAKER_LOCAL_CPPDEFINES(-DGPU_VOXELS_EXPORT_SYMBOLS -Wno-unknown-pragmas)
ICMAKER_GLOBAL_CPPDEFINES(-D_IC_BUILDER_GPU_VOXELS_EXAMPLES_HEIGHTMAP_LOADER_)
ICMAKER_INCLUDE_DIRECTORIES(${GPU_VOXELS_INCLUDE_DIRS})

ICMAKER_INTERNAL_DEPENDENCIES(
  icl_core
  icl_core_config
  icl_core_logging
  gpu_voxels
  )

ICMAKER_EXTERNAL_DEPENDENCIES(
  CUDA
  )

ICMAKER_BUILD_PROGRAM()

#------------- Example Program for the usage of gpu_voxels ------------
ICMAKER_SET("swept_volume_vs_environment" IDE_FOLDER ${EXAMPLES_IDE_FOLDER})

ICMAKER_ADD_HEADERS(
  )

ICMAKER_ADD_SOURCES(
  SweptVolumeVsEnvironment.cpp
  )

ICMAKER_ADD_CUDA_FILES(
  )

ICMAKER_LOCAL_CPPDEFINES(-DGPU_VOXELS_EXPORT_SYMBOLS -Wno-unknown-pragmas)
ICMAKER_GLOBAL_CPPDEFINES(-D_IC_BUILDER_GPU_VOXELS_EXAMPLES_SV_VS_ENV_)
ICMAKER_INCLUDE_DIRECTORIES(${GPU_VOXELS_INCLUDE_DIRS})

ICMAKER_INTERNAL_DEPENDENCIES(
  icl_core
  icl_core_config
  icl_core_logging
  gpu_voxels
  )

ICMAKER_EXTERNAL_DEPENDENCIES(
  CUDA
  OpenNI
  PCL
  )

ICMAKER_BUILD_PROGRAM()

#------------- Example Program sandbox ------------
ICMAKER_SET("sandbox" IDE_FOLDER ${EXAMPLES_IDE_FOLDER})

ICMAKER_ADD_HEADERS(
  )

ICMAKER_ADD_SOURCES(
  Sandbox.cpp
  )

ICMAKER_ADD_CUDA_FILES(
  )

ICMAKER_LOCAL_CPPDEFINES(-DGPU_VOXELS_EXPORT_SYMBOLS -Wno-unknown-pragmas)
ICMAKER_GLOBAL_CPPDEFINES(-D_IC_BUILDER_GPU_VOXELS_EXAMPLES_SANDBOX_)
ICMAKER_INCLUDE_DIRECTORIES(${GPU_VOXELS_INCLUDE_DIRS})

ICMAKER_INTERNAL_DEPENDENCIES(
  icl_core
  icl_core_config
  icl_core_logging
  gpu_voxels
  )

ICMAKER_EXTERNAL_DEPENDENCIES(
  CUDA
  )

ICMAKER_BUILD_PROGRAM()

#------------- Example Program to deal with probabilistic voxels ------------
ICMAKER_SET("prob_voxels" IDE_FOLDER ${EXAMPLES_IDE_FOLDER})

ICMAKER_ADD_HEADERS(
  )

ICMAKER_ADD_SOURCES(
  ProbVoxels.cpp
  )

ICMAKER_ADD_CUDA_FILES(
  )

ICMAKER_LOCAL_CPPDEFINES(-DGPU_VOXELS_EXPORT_SYMBOLS -Wno-unknown-pragmas)
ICMAKER_GLOBAL_CPPDEFINES(-D_IC_BUILDER_GPU_VOXELS_EXAMPLES_VOXELMAP_SANDBOX_)
ICMAKER_INCLUDE_DIRECTORIES(${GPU_VOXELS_INCLUDE_DIRS})

ICMAKER_INTERNAL_DEPENDENCIES(
  icl_core
  icl_core_config
  icl_core_logging
  gpu_voxels
  Boost_SYSTEM
  )

ICMAKER_EXTERNAL_DEPENDENCIES(
  CUDA
  )

ICMAKER_BUILD_PROGRAM()


#------------- Example Program to create a distance map from a prob map ------------
ICMAKER_SET("prob2distmap" IDE_FOLDER ${EXAMPLES_IDE_FOLDER})

ICMAKER_ADD_HEADERS(
  )

ICMAKER_ADD_SOURCES(
  ProbMap2DistMap.cpp
  )

ICMAKER_ADD_CUDA_FILES(
  )

ICMAKER_LOCAL_CPPDEFINES(-DGPU_VOXELS_EXPORT_SYMBOLS -Wno-unknown-pragmas)
ICMAKER_GLOBAL_CPPDEFINES(-D_IC_BUILDER_GPU_VOXELS_EXAMPLES_VOXELMAP_SANDBOX_)
ICMAKER_INCLUDE_DIRECTORIES(${GPU_VOXELS_INCLUDE_DIRS})

ICMAKER_INTERNAL_DEPENDENCIES(
  icl_core
  icl_core_config
  icl_core_logging
  gpu_voxels
  Boost_SYSTEM
  )

ICMAKER_EXTERNAL_DEPENDENCIES(
  CUDA
  )

ICMAKER_BUILD_PROGRAM()

#------------- Example Program about loading URDFs ------------
ICMAKER_SET("urdf_loader" IDE_FOLDER ${EXAMPLES_IDE_FOLDER})

ICMAKER_ADD_HEADERS(
  )

ICMAKER_ADD_SOURCES(
  URDF_Loader.cpp
  )

ICMAKER_ADD_CUDA_FILES(
  )

ICMAKER_LOCAL_CPPDEFINES(-DGPU_VOXELS_EXPORT_SYMBOLS -Wno-unknown-pragmas)
ICMAKER_GLOBAL_CPPDEFINES(-D_IC_BUILDER_GPU_VOXELS_EXAMPLES_URDF_LOADER_)
ICMAKER_INCLUDE_DIRECTORIES(${GPU_VOXELS_INCLUDE_DIRS})

ICMAKER_INTERNAL_DEPENDENCIES(
  icl_core
  icl_core_config
  icl_core_logging
  gpu_voxels
  gpu_voxels_urdf_robot
  )

ICMAKER_EXTERNAL_DEPENDENCIES(
  CUDA
  )

ICMAKER_BUILD_PROGRAM()

#------------- Example Program about loading URDFs and checking for self collisions ------------
ICMAKER_SET("urdf_loader_self_coll" IDE_FOLDER ${EXAMPLES_IDE_FOLDER})

ICMAKER_ADD_HEADERS(
  )

ICMAKER_ADD_SOURCES(
  URDF_Loader_Selfcoll.cpp
  )

ICMAKER_ADD_CUDA_FILES(
  )

ICMAKER_LOCAL_CPPDEFINES(-DGPU_VOXELS_EXPORT_SYMBOLS -Wno-unknown-pragmas)
ICMAKER_GLOBAL_CPPDEFINES(-D_IC_BUILDER_GPU_VOXELS_EXAMPLES_URDF_LOADER_)
ICMAKER_INCLUDE_DIRECTORIES(${GPU_VOXELS_INCLUDE_DIRS})

ICMAKER_INTERNAL_DEPENDENCIES(
  icl_core
  icl_core_config
  icl_core_logging
  gpu_voxels
  gpu_voxels_urdf_robot
  )

ICMAKER_EXTERNAL_DEPENDENCIES(
  CUDA
  )

ICMAKER_BUILD_PROGRAM()

#------------- Example Program about URDF together with ROS ------------

ICMAKER_SET("urdf_loader_ros_listener" IDE_FOLDER ${EXAMPLES_IDE_FOLDER})

ICMAKER_ADD_HEADERS(
  )

ICMAKER_ADD_SOURCES(
  URDF_Loader_ROS_listener.cpp
  )

ICMAKER_ADD_CUDA_FILES(
  )

ICMAKER_LOCAL_CPPDEFINES(-DGPU_VOXELS_EXPORT_SYMBOLS -Wno-unknown-pragmas)
ICMAKER_GLOBAL_CPPDEFINES(-D_IC_BUILDER_GPU_VOXELS_EXAMPLES_URDF_LOADER_ROS_)
ICMAKER_INCLUDE_DIRECTORIES(${GPU_VOXELS_INCLUDE_DIRS})

ICMAKER_INTERNAL_DEPENDENCIES(
  icl_core
  icl_core_config
  icl_core_logging
  gpu_voxels
  gpu_voxels_urdf_robot
  )

ICMAKER_EXTERNAL_DEPENDENCIES(
  ROS
  CUDA
  )

ICMAKER_BUILD_PROGRAM()

#------------- Example Program about ROS TF interfacing ------------
ICMAKER_SET("tf_interface" IDE_FOLDER ${EXAMPLES_IDE_FOLDER})

ICMAKER_ADD_HEADERS(
  )

ICMAKER_ADD_SOURCES(
  tfInterface.cpp
  )

ICMAKER_ADD_CUDA_FILES(
  )

ICMAKER_LOCAL_CPPDEFINES(-DGPU_VOXELS_EXPORT_SYMBOLS -Wno-unknown-pragmas)
ICMAKER_GLOBAL_CPPDEFINES(-D_IC_BUILDER_GPU_VOXELS_EXAMPLES_TF_INTERFACE_)
ICMAKER_INCLUDE_DIRECTORIES(${GPU_VOXELS_INCLUDE_DIRS})

ICMAKER_INTERNAL_DEPENDENCIES(
  icl_core
  icl_core_config
  icl_core_logging
  gpu_voxels
  )

ICMAKER_EXTERNAL_DEPENDENCIES(
  ROS
  CUDA
  )

ICMAKER_BUILD_PROGRAM()

#------------- Example Program for the usage of gpu_voxels ------------
ICMAKER_SET("robot_vs_environment" IDE_FOLDER ${EXAMPLES_IDE_FOLDER})

ICMAKER_ADD_HEADERS(
  )

ICMAKER_ADD_SOURCES(
  RobotVsEnvironment.cpp
  )

ICMAKER_ADD_CUDA_FILES(
  )

ICMAKER_LOCAL_CPPDEFINES(-DGPU_VOXELS_EXPORT_SYMBOLS -Wno-unknown-pragmas)
ICMAKER_GLOBAL_CPPDEFINES(-D_IC_BUILDER_GPU_VOXELS_EXAMPLES_ROBOT_VS_ENV_)
ICMAKER_INCLUDE_DIRECTORIES(${GPU_VOXELS_INCLUDE_DIRS})

ICMAKER_INTERNAL_DEPENDENCIES(
  icl_core
  icl_core_config
  icl_core_logging
  gpu_voxels
  )

ICMAKER_EXTERNAL_DEPENDENCIES(
  CUDA
  OpenNI
  PCL
  )

ICMAKER_BUILD_PROGRAM()


#------------- Example Program voxellist sandbox ------------
ICMAKER_SET("voxellist_sandbox" IDE_FOLDER ${EXAMPLES_IDE_FOLDER})

ICMAKER_ADD_HEADERS(
  )

ICMAKER_ADD_SOURCES(
  VoxelListSandbox.cpp
  )

ICMAKER_ADD_CUDA_FILES(
  )

ICMAKER_LOCAL_CPPDEFINES(-DGPU_VOXELS_EXPORT_SYMBOLS -Wno-unknown-pragmas)
ICMAKER_GLOBAL_CPPDEFINES(-D_IC_BUILDER_GPU_VOXELS_EXAMPLES_VOXELLIST_SANDBOX_)
ICMAKER_INCLUDE_DIRECTORIES(${GPU_VOXELS_INCLUDE_DIRS})

ICMAKER_INTERNAL_DEPENDENCIES(
  icl_core
  icl_core_config
  icl_core_logging
  gpu_voxels
  Boost_SYSTEM
  PCL
  )

ICMAKER_EXTERNAL_DEPENDENCIES(
  CUDA
  )

ICMAKER_BUILD_PROGRAM()



#------------- Example Program voxelmap sandbox ------------
ICMAKER_SET("voxelmap_sandbox" IDE_FOLDER ${EXAMPLES_IDE_FOLDER})

ICMAKER_ADD_HEADERS(
  )

ICMAKER_ADD_SOURCES(
  VoxelMapSandbox.cpp
  )

ICMAKER_ADD_CUDA_FILES(
  )

ICMAKER_LOCAL_CPPDEFINES(-DGPU_VOXELS_EXPORT_SYMBOLS -Wno-unknown-pragmas)
ICMAKER_GLOBAL_CPPDEFINES(-D_IC_BUILDER_GPU_VOXELS_EXAMPLES_VOXELMAP_SANDBOX_)
ICMAKER_INCLUDE_DIRECTORIES(${GPU_VOXELS_INCLUDE_DIRS})

ICMAKER_INTERNAL_DEPENDENCIES(
  icl_core
  icl_core_config
  icl_core_logging
  gpu_voxels
  Boost_SYSTEM
  PCL
  )

ICMAKER_EXTERNAL_DEPENDENCIES(
  CUDA
  )

ICMAKER_BUILD_PROGRAM()

#------------- Example Program raycasting_sensor_example ------------
ICMAKER_SET("raycasting_sensor_example" IDE_FOLDER ${EXAMPLES_IDE_FOLDER})

ICMAKER_ADD_HEADERS(
  )

ICMAKER_ADD_SOURCES(
  RaycastingSensorExample.cpp
  )

ICMAKER_ADD_CUDA_FILES(
  )

ICMAKER_LOCAL_CPPDEFINES(-DGPU_VOXELS_EXPORT_SYMBOLS -Wno-unknown-pragmas)
ICMAKER_GLOBAL_CPPDEFINES(-D_IC_BUILDER_GPU_VOXELS_EXAMPLES_VOXELMAP_SANDBOX_)
ICMAKER_INCLUDE_DIRECTORIES(${GPU_VOXELS_INCLUDE_DIRS})

ICMAKER_INTERNAL_DEPENDENCIES(
  icl_core
  icl_core_config
  icl_core_logging
  gpu_voxels
  Boost_SYSTEM
  )


ICMAKER_EXTERNAL_DEPENDENCIES(
  CUDA
  )

ICMAKER_BUILD_PROGRAM()


#------------- Example Program distance_voxel_test ------------
ICMAKER_SET("distance_voxel_test" IDE_FOLDER ${EXAMPLES_IDE_FOLDER})
add_definitions(-DIC_PERFORMANCE_MONITOR)

ICMAKER_ADD_HEADERS(
  )

ICMAKER_ADD_SOURCES(
  DistanceVoxelTest.cpp
  )

ICMAKER_ADD_CUDA_FILES(
  )

ICMAKER_LOCAL_CPPDEFINES(-DGPU_VOXELS_EXPORT_SYMBOLS -Wno-unknown-pragmas)
ICMAKER_GLOBAL_CPPDEFINES(-D_IC_BUILDER_GPU_VOXELS_EXAMPLES_DISTANCE_VOXEL_TEST_)
ICMAKER_INCLUDE_DIRECTORIES(${GPU_VOXELS_INCLUDE_DIRS})

ICMAKER_INTERNAL_DEPENDENCIES(
  gpu_voxels
  )

ICMAKER_EXTERNAL_DEPENDENCIES(
  icl_core
  icl_core_config
  icl_core_logging
  icl_core_performance_monitor
  Boost_SYSTEM
  CUDA
  )

ICMAKER_BUILD_PROGRAM()

#------------- Example Program distance_kinect_demo ------------
ICMAKER_SET("distance_kinect_demo" IDE_FOLDER ${EXAMPLES_IDE_FOLDER})
add_definitions(-DIC_PERFORMANCE_MONITOR)

ICMAKER_ADD_HEADERS(
  )

ICMAKER_ADD_SOURCES(
  DistanceKinectDemo.cpp
  )

ICMAKER_ADD_CUDA_FILES(
  )

ICMAKER_LOCAL_CPPDEFINES(-DGPU_VOXELS_EXPORT_SYMBOLS -Wno-unknown-pragmas)
ICMAKER_GLOBAL_CPPDEFINES(-D_IC_BUILDER_GPU_VOXELS_EXAMPLES_DISTANCE_KINECT_DEMO_)
ICMAKER_INCLUDE_DIRECTORIES(${GPU_VOXELS_INCLUDE_DIRS})

ICMAKER_INTERNAL_DEPENDENCIES(
  gpu_voxels
  )

ICMAKER_EXTERNAL_DEPENDENCIES(
  icl_core
  icl_core_config
  icl_core_logging
  icl_core_performance_monitor
  Boost_SYSTEM
  CUDA
  OpenNI
  PCL
  )

ICMAKER_BUILD_PROGRAM()

#------------- Example Program for the two primitiveArray APIs ------------
ICMAKER_SET("primitivearraytest" IDE_FOLDER ${EXAMPLES_IDE_FOLDER})

ICMAKER_ADD_HEADERS(

  )

ICMAKER_ADD_SOURCES(
  PrimitiveArrayTest.cpp
  )

ICMAKER_ADD_CUDA_FILES(
  )

ICMAKER_LOCAL_CPPDEFINES(-DGPU_VOXELS_EXPORT_SYMBOLS -Wno-unknown-pragmas)
ICMAKER_GLOBAL_CPPDEFINES(-D_IC_BUILDER_GPU_VOXELS_EXAMPLES_REFACTORINGTEST_)
ICMAKER_INCLUDE_DIRECTORIES(${GPU_VOXELS_INCLUDE_DIRS})

ICMAKER_INTERNAL_DEPENDENCIES(
  icl_core
  icl_core_config
  icl_core_logging
  gpu_voxels
  )

ICMAKER_EXTERNAL_DEPENDENCIES(

  )

ICMAKER_BUILD_PROGRAM()

#------------- Example Program for the usage of gpu_voxels ------------
ICMAKER_SET("counting_sandbox" IDE_FOLDER ${EXAMPLES_IDE_FOLDER})

ICMAKER_ADD_HEADERS(
  )

ICMAKER_ADD_SOURCES(
  VoxelListCountingSandbox.cpp
  )

ICMAKER_ADD_CUDA_FILES(
  )

ICMAKER_LOCAL_CPPDEFINES(-DGPU_VOXELS_EXPORT_SYMBOLS -Wno-unknown-pragmas)
ICMAKER_GLOBAL_CPPDEFINES(-D_IC_BUILDER_GPU_VOXELS_EXAMPLES_COLLISION_)
ICMAKER_INCLUDE_DIRECTORIES(${GPU_VOXELS_INCLUDE_DIRS})

ICMAKER_INTERNAL_DEPENDENCIES(
  icl_core
  icl_core_config
  icl_core_logging
  gpu_voxels
  )

ICMAKER_EXTERNAL_DEPENDENCIES(
  CUDA
  )

ICMAKER_BUILD_PROGRAM()

#------------- Example Program for the usage of gpu_voxels ------------
ICMAKER_SET("counting_voxellist" IDE_FOLDER ${EXAMPLES_IDE_FOLDER})

ICMAKER_ADD_HEADERS(
  )

ICMAKER_ADD_SOURCES(
  CountingVoxelList.cpp
  )

ICMAKER_ADD_CUDA_FILES(
  )

ICMAKER_LOCAL_CPPDEFINES(-DGPU_VOXELS_EXPORT_SYMBOLS -Wno-unknown-pragmas)
ICMAKER_GLOBAL_CPPDEFINES(-D_IC_BUILDER_GPU_VOXELS_EXAMPLES_COLLISION_)
ICMAKER_INCLUDE_DIRECTORIES(${GPU_VOXELS_INCLUDE_DIRS})

ICMAKER_INTERNAL_DEPENDENCIES(
  icl_core
  icl_core_config
  icl_core_logging
  gpu_voxels
  )

ICMAKER_EXTERNAL_DEPENDENCIES(
  CUDA
  )

ICMAKER_BUILD_PROGRAM()


#------------- Example Program using showing the boundary checks for inserting into a map ------------
ICMAKER_SET("geometrygeneration" IDE_FOLDER ${EXAMPLES_IDE_FOLDER})

ICMAKER_ADD_HEADERS(
  )

ICMAKER_ADD_SOURCES(
  GeometryGeneration.cpp
  )

ICMAKER_ADD_CUDA_FILES(
  )

ICMAKER_LOCAL_CPPDEFINES(-DGPU_VOXELS_EXPORT_SYMBOLS -Wno-unknown-pragmas)
ICMAKER_GLOBAL_CPPDEFINES(-D_IC_BUILDER_GPU_VOXELS_EXAMPLES_BOUNDCHECK_)
ICMAKER_INCLUDE_DIRECTORIES(${GPU_VOXELS_INCLUDE_DIRS})

ICMAKER_INTERNAL_DEPENDENCIES(
  icl_core
  icl_core_config
  icl_core_logging
  gpu_voxels
  gpu_voxels_distance_map_converter
  )

ICMAKER_EXTERNAL_DEPENDENCIES(
  CUDA
  )

ICMAKER_BUILD_PROGRAM()


#------------- adding examples in subdirectories ------------
ADD_SUBDIRECTORY(swept_fitter)