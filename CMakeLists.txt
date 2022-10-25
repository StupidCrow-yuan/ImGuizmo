set(SOURCE_FILES)
foreach( DIR ${CMAKE_CURRENT_LIST_DIR} )
    file(GLOB_RECURSE TEMP_FILES  ${DIR}/ImGuizmo.cpp ${DIR}/ImGuizmo.h)
    list(APPEND SOURCE_FILES ${TEMP_FILES})
endforeach()

target_sources(${EXE_NAME} PRIVATE ${SOURCE_FILES})