PROJECT(AdminManual_DOC NONE)

ADD_LATEX_DOCUMENT(hypha-admin-manual.tex
 	IMAGE_DIRS .
	DEFAULT_PDF MANGLE_TARGET_NAMES
  )
INSTALL(FILES ${CMAKE_CURRENT_BINARY_DIR}/hypha-admin-manual.pdf
  DESTINATION /usr/share/doc/Hypha )

