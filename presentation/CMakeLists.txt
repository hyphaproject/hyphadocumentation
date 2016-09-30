PROJECT(HyphaPresentation_DOC NONE)

ADD_LATEX_DOCUMENT(hypha-presentation.tex
	INPUTS Content.tex
 	IMAGE_DIRS .
	DEFAULT_PDF MANGLE_TARGET_NAMES
  )
INSTALL(FILES ${CMAKE_CURRENT_BINARY_DIR}/hypha-presentation.pdf
  DESTINATION /usr/share/doc/Hypha )
