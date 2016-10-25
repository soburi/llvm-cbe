set(LLVM_LINK_COMPONENTS
  ${LLVM_TARGETS_TO_BUILD}
  BitReader
  AsmParser
  IRReader
  CBackendCodeGen
  CBackendInfo
  )

add_llvm_tool(llvm-cbe
  llvm-cbe.cpp
  )
export_executable_symbols(llvm-cbe)
