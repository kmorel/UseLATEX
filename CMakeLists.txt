cmake_minimum_required(VERSION 2.8.4)

project(UseLATEX_DOC NONE)

include(UseLATEX.cmake)

# Note that normally CMakeLists.txt would not be considered an
# input to the document, but in this special case of documenting
# UseLATEX.cmake the contents of this file is actually included
# in the document.
# USE_BIBLATEX enables the use of biblatex/biber as an alternative
# to bibtex. Bibtex remains the default if USE_BIBLATEX is not specified.
# Biber is the only backend supported for use with biblatex, although it
# is possible to manually change this in UseLATEX.cmake.
add_latex_document(UseLATEX.tex
  INPUTS CMakeLists.txt
  USE_BIBLATEX
  )
