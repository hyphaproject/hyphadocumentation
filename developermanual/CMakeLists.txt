PROJECT(DeveloperManual_DOC NONE)

ADD_LATEX_DOCUMENT(hypha-developer-manual.tex
 	IMAGE_DIRS .
	DEFAULT_PDF MANGLE_TARGET_NAMES
  )
INSTALL(FILES ${CMAKE_CURRENT_BINARY_DIR}/hypha-developer-manual.pdf
  DESTINATION /usr/share/doc/Hypha )
