include $(top_srcdir)/build/vars.build.mk

geanyplugins_LTLIBRARIES = geanyprj.la

geanyprj_la_SOURCES = geanyprj.c \
	geanyprj.h \
	menu.c \
	project.c \
	sidebar.c \
	utils.c \
	xproject.c

geanyprj_la_CFLAGS = $(AM_CFLAGS)
geanyprj_la_LIBADD = $(COMMONLIBS)

AM_CPPCHECKFLAGS = --suppress='constStatement:*'
AM_CPPCHECKFLAGS += --suppress='memleak:utils.c:72'

include $(top_srcdir)/build/cppcheck.mk
