CMAKE_MINIMUM_REQUIRED(VERSION 3.0.0)

PROJECT(DeveloperManual_DOC NONE)

INCLUDE(UseLATEX.cmake)

ADD_LATEX_DOCUMENT(hypha-developer-manual.tex
 	IMAGE_DIRS .
	DEFAULT_PDF
  )
INSTALL(FILES ${CMAKE_CURRENT_BINARY_DIR}/hypha-developer-manual.pdf
  DESTINATION /usr/share/doc/Hypha )
