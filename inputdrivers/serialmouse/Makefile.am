## Makefile.am for DirectFB/inputdrivers/serialmouse

INCLUDES = \
	-I$(top_builddir)/include	\
	-I$(top_builddir)/lib	\
	-I$(top_srcdir)/include	\
	-I$(top_srcdir)/lib	\
	-I$(top_srcdir)/src

serialmouse_LTLIBRARIES = libdirectfb_serialmouse.la

if BUILD_STATIC
serialmouse_DATA = $(serialmouse_LTLIBRARIES:.la=.o)
endif

serialmousedir = $(MODULEDIR)/inputdrivers

libdirectfb_serialmouse_la_SOURCES = serialmouse.c

libdirectfb_serialmouse_la_LDFLAGS = \
	-module			\
	-avoid-version		\
	$(DFB_LDFLAGS)

libdirectfb_serialmouse_la_LIBADD = \
	$(top_builddir)/lib/direct/libdirect.la \
	$(top_builddir)/src/libdirectfb.la


include $(top_srcdir)/rules/libobject.make
	
