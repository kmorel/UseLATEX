PROJECT(UseLATEX_DOC NONE)

INCLUDE(UseLATEX.cmake)

# Note that normally neither CMakeLists.txt nor UseLATEX.cmake
# would be considered inputs to the document, but in this
# special case (of documenting UseLATEX.cmake) the contents of
# these files are actually included in the document.
ADD_LATEX_DOCUMENT(UseLATEX.tex
  INPUTS CMakeLists.txt UseLATEX.cmake
  )
