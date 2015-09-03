cmake_minimum_required(VERSION 2.8.4)

project(MultiIndex NONE)

include(../../UseLATEX.cmake)

add_latex_document(SingleIndex.tex
  USE_INDEX
  )

add_latex_document(MultiIndex.tex
  USE_INDEX
  INDEX_NAMES terms people
  )
