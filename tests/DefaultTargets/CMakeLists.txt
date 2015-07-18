cmake_minimum_required(VERSION 2.8.4)

project(DefaultTargets NONE)

include(../../UseLATEX.cmake)

add_latex_document(DefaultDvi.tex FORCE_DVI)
add_latex_document(DefaultPdf.tex FORCE_PDF)
add_latex_document(DefaultHtml.tex FORCE_HTML)
add_latex_document(NoDefault.tex EXCLUDE_FROM_ALL)
