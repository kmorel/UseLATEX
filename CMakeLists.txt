CMAKE_MINIMUM_REQUIRED(VERSION 2.6)

PROJECT(UseLATEX_DOC NONE)

INCLUDE(UseLATEX.cmake)

# Note that normally CMakeLists.txt would not be considered an
# input to the document, but in this special case of documenting
# UseLATEX.cmake the contents of this file is actually included
# in the document.
ADD_LATEX_DOCUMENT(UseLATEX.tex
  INPUTS CMakeLists.txt
  )
