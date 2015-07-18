cmake_minimum_required(VERSION 2.8.4)

project(ImageTypes NONE)

include(../../UseLATEX.cmake)

add_latex_document(ImageTypes.tex
  IMAGE_DIRS images
  )
