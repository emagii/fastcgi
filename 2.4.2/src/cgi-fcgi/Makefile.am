# $Id: Makefile.am,v 1.4 2001/12/22 03:16:22 robs Exp $
bin_PROGRAMS     = cgi-fcgi

ACLOCAL_AMFLAGS         = ${ACLOCAL_FLAGS} '-Im4'

INCLUDEDIR  = ../include
AM_CPPFLAGS    = -I$(top_srcdir)/include

INCLUDE_FILES   = $(INCLUDEDIR)/fastcgi.h  \
		  $(INCLUDEDIR)/fcgiapp.h  \
		  $(INCLUDEDIR)/fcgimisc.h

LIBDIR      = ../libfcgi
LIBFCGI     = $(LIBDIR)/libfcgi.la

LDADD = $(LIBFCGI)
cgi_fcgi_SOURCES = $(INCLUDE_FILES) cgi-fcgi.c
