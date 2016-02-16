cmake_minimum_required(VERSION 2.8.4)

project(Bibliography NONE)

include(../../UseLATEX.cmake)

add_latex_document(DocWithBib.tex
  BIBFILES References.bib
  )

add_latex_document(DocWithBibLatex.tex
  BIBFILES References.bib
  USE_BIBLATEX
  )
