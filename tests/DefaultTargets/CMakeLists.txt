cmake_minimum_required(VERSION 2.8)

project(DefaultTargets NONE)

include(../../UseLATEX.cmake)

add_latex_document(DefaultDvi.tex FORCE_DVI MANGLE_TARGET_NAMES)
add_latex_document(DefaultPdf.tex FORCE_PDF MANGLE_TARGET_NAMES)
add_latex_document(DefaultHtml.tex FORCE_HTML MANGLE_TARGET_NAMES)
add_latex_document(NoDefault.tex EXCLUDE_FROM_ALL MANGLE_TARGET_NAMES)
