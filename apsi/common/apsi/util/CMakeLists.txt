# Source files in this directory
set(APSI_SOURCE_FILES ${APSI_SOURCE_FILES}
    ${CMAKE_CURRENT_LIST_DIR}/interpolate.cpp
    ${CMAKE_CURRENT_LIST_DIR}/label_encryptor.cpp
    ${CMAKE_CURRENT_LIST_DIR}/db_encoding.cpp
    ${CMAKE_CURRENT_LIST_DIR}/stopwatch.cpp
    ${CMAKE_CURRENT_LIST_DIR}/utils.cpp
)

# Add header files for installation
install(
    FILES
        ${CMAKE_CURRENT_LIST_DIR}/interpolate.h
        ${CMAKE_CURRENT_LIST_DIR}/label_encryptor.h
        ${CMAKE_CURRENT_LIST_DIR}/db_encoding.h
        ${CMAKE_CURRENT_LIST_DIR}/stopwatch.h
        ${CMAKE_CURRENT_LIST_DIR}/thread_pool.h
        ${CMAKE_CURRENT_LIST_DIR}/utils.h
    DESTINATION
        ${APSI_INCLUDES_INSTALL_DIR}/apsi/util
)

set(APSI_SOURCE_FILES ${APSI_SOURCE_FILES} PARENT_SCOPE)
