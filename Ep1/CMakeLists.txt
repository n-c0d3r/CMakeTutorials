cmake_minimum_required(VERSION 3.24.0)



project(Ep1)



set_property(GLOBAL PROPERTY USE_FOLDERS ON)



file(GLOB SourcePrivateGroup
    "Source/Private/*.cpp"
)

source_group("Source\\Private" FILES ${SourcePrivateGroup})



add_executable(HelloWorld 
    ${SourcePrivateGroup}
)