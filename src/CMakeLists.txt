set(CMAKE_CXX_FLAGS "-std=c++14")

set(CPP_PARSER_SOURCES
    main.cpp
)

#TODO Find LLVM and CLang LibTooling

set(LLVM_INCLUDE_DIR "${VENDOR_DIR}/llvm/include")
set(CLANG_INCLUDE_DIR "${VENDOR_DIR}/llvm/tools/clang/include" )


include_directories( ${LLVM_INCLUDE_DIR} ${CLANG_INCLUDE_DIR} )

add_executable(cpp_parserd ${CPP_PARSER_SOURCES})

