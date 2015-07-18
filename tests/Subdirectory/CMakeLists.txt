cmake_minimum_required(VERSION 2.8.4)

project(Subdirectory NONE)

include(../../UseLATEX.cmake)

add_latex_document(subdir/Subdirectory.tex
  IMAGE_DIRS subdir/images
  INPUTS subdir/IncludedFile.tex
  )
