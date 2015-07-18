cmake_minimum_required(VERSION 2.8.4)

project(MultiDotFilename NONE)

include(../../UseLATEX.cmake)

add_latex_document(multi.dot.filename.tex
  BIBFILES multi.dot.filename.bib
  IMAGES my.image.eps
  )
