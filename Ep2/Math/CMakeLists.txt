


file(GLOB SourcePrivateGroup
    "Source/Math/Private/*.cpp"
)

source_group("Source\\Private" FILES ${SourcePrivateGroup})



file(GLOB SourcePublicGroup
    "Source/Math/Public/*.h"
)

source_group("Source\\Public" FILES ${SourcePublicGroup})



add_library(Math 
    ${SourcePrivateGroup}
    ${SourcePublicGroup}
)