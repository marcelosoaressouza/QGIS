ADD_SUBDIRECTORY(core)
ADD_SUBDIRECTORY(analysis)
ADD_SUBDIRECTORY(ui)
ADD_SUBDIRECTORY(gui)
ADD_SUBDIRECTORY(providers)
ADD_SUBDIRECTORY(crssync)

IF (WITH_DESKTOP)
  ADD_SUBDIRECTORY(app)
  ADD_SUBDIRECTORY(helpviewer)
  ADD_SUBDIRECTORY(browser)
  ADD_SUBDIRECTORY(plugins)
ENDIF(WITH_DESKTOP)

IF (WITH_BINDINGS)
  ADD_SUBDIRECTORY(python)
ENDIF (WITH_BINDINGS)

IF (WITH_MAPSERVER)
  ADD_SUBDIRECTORY(mapserver)  # TODO: enable again once compilation is fixed
ENDIF (WITH_MAPSERVER)

IF (WITH_ASTYLE)
  ADD_SUBDIRECTORY(astyle)
ENDIF(WITH_ASTYLE)
