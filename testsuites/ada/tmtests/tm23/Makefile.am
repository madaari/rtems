include $(RTEMS_ROOT)/make/custom/@RTEMS_BSP@.cfg
include $(top_srcdir)/../automake/compile.am

include $(top_srcdir)/ada.am

noinst_PROGRAMS = ada_tm23
ada_tm23_SOURCES = tm23.adb config.h tmtest.adb tmtest.ads
ada_tm23_SOURCES += ../../support/init.c

ada_tm23$(EXEEXT): tm23.adb init.$(OBJEXT)
	$(GNATCOMPILE) -margs -a $< -o $@

include $(top_srcdir)/../automake/local.am
