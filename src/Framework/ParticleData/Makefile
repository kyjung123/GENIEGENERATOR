#
# Makefile for GENIE Neutrino Generator
#
# Costas Andreopoulos <c.andreopoulos \at cern.ch>
#

SHELL    = /bin/sh
NAME     = all
MAKEFILE = Makefile

# Include machine specific flags and locations (inc. files & libs)
#
include $(GENIE)/src/make/Make.include

PACKAGE           = Framework/ParticleData
PACKAGE_ABBREV    = FwParDat
DICTIONARY        = _ROOT_DICT_$(PACKAGE_ABBREV)
LIBNAME           = libG$(PACKAGE_ABBREV)
EXTRA_EXT_LIBS    = -L$(GENIE_LIB_PATH) -lGFwMsg

all     : rootcint lib lib-link
install : install-inc install-lib

# Include standard package makefile targets
#
include $(GENIE)/src/make/Make.std-package-targets

FORCE:
