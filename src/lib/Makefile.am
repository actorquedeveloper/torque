include $(top_srcdir)/buildutils/config.mk

SUBDIRS = Libattr Libcmds Libcsv Libdis Libifl Liblog Libnet Libpbs Libsite Libutils

CHECK_DIR = test

DIST_SUBDIRS = Libattr Libcmds Libcsv Libdis Libifl Liblog Libnet Libpbs Libsite Libutils

if HAVE_CHECK
cleancheck:
	@for dir in $(SUBDIRS) $(CHECK_DIR); do (cd $$dir && $(MAKE) cleancheck); done

check:
	@for dir in $(SUBDIRS) $(CHECK_DIR); do (cd $$dir && $(MAKE) $(MAKECMDGOALS)); done
endif
