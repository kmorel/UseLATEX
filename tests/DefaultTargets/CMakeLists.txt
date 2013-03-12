cmake_minimum_required(VERSION 2.8)

project(DefaultTargets NONE)

include(../../UseLATEX.cmake)

add_latex_document(DefaultDvi.tex MANGLE_TARGET_NAMES)
add_latex_document(DefaultPdf.tex DEFAULT_PDF MANGLE_TARGET_NAMES)
add_latex_document(DefaultSafePdf.tex DEFAULT_SAFEPDF MANGLE_TARGET_NAMES)
add_latex_document(DefaultPs.tex DEFAULT_PS MANGLE_TARGET_NAMES)
add_latex_document(NoDefault.tex NO_DEFAULT MANGLE_TARGET_NAMES)
