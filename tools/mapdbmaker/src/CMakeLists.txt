AUX_SOURCE_DIRECTORY(. MAPDBMAKER)
ADD_EXECUTABLE(mapdbmaker ${MAPDBMAKER})
ADD_DEPENDENCIES(mapdbmaker mir2x_3rds)

TARGET_INCLUDE_DIRECTORIES(mapdbmaker PRIVATE ${MIR2X_COMMON_SOURCE_DIR})
TARGET_INCLUDE_DIRECTORIES(mapdbmaker PRIVATE ${CMAKE_CURRENT_BINARY_DIR})
TARGET_INCLUDE_DIRECTORIES(mapdbmaker PRIVATE ${CMAKE_CURRENT_LIST_DIR})

TARGET_LINK_LIBRARIES(mapdbmaker common)
