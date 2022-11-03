


file(GLOB SourcePrivateGroup
    "Source/MainProgram/Private/*.cpp"
)

source_group("Source\\Private" FILES ${SourcePrivateGroup})



add_executable(MainProgram 
    ${SourcePrivateGroup}
)



target_include_directories(MainProgram
    PUBLIC ../Math/Source/
)



target_link_directories(MainProgram
    PRIVATE ../Build/Math/${CMAKE_BUILD_TYPE}/
)



target_link_libraries(MainProgram
    Math
)



add_dependencies(MainProgram Math)