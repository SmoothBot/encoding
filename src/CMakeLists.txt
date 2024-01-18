add_library (
  EncodingLib 
  Encoding.h
  Encoding.cpp
)

install (TARGETS EncodingLib DESTINATION bin)
install (FILES Encoding.h DESTINATION include)
