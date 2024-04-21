

message(INFO "<MS>")
message(INFO "<MS> ADS1115_WE >>")
message(INFO "<MS>")
message(INFO "<MS> CMAKE_CURRENT_SOURCE_DIR: ${CMAKE_CURRENT_SOURCE_DIR}")


set(ADS1115_WE_SRCS src/ADS1115_WE.cpp)
set(ADS1115_WE_INCL ${CMAKE_CURRENT_SOURCE_DIR}/src)
set(ADS1115_WE_REQU 
    arduino 
    )

idf_component_register(
    INCLUDE_DIRS ${ADS1115_WE_INCL} 
    SRCS ${ADS1115_WE_SRCS}
    REQUIRES ${ADS1115_WE_REQU}
    )

message(INFO "<MS>")
message(INFO "<MS> ADS1115_WE <<")
message(INFO "<MS>")
