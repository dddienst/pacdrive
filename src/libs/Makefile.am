# src/libs/Makefile.am

AM_CFLAGS = $(JSON_CFLAGS) $(LIBUSB_CFLAGS)
AM_LDFLAGS = $(JSON_LIBS) $(LIBUSB_LIBS)


lib_LTLIBRARIES = libultimarc.la
libultimarc_la_SOURCES = ultimarc.c ipac.c ultistik.c pacLED.c common.c pacdrive.c ipacultimate.c ipacseries.c ulboard.c usbbutton.c servostik.c uhid.c ipac.h ultistik.h pacLED.h common.h pacdrive.h ipacultimate.h dbg.h ipacseries.h usbbutton.h servostik.h uhid.h
libultimarc_la_LDFLAGS = $(AM_LDFLAGS) -version-info 1:1:0

otherincludedir = $(includedir)/ultimarc
otherinclude_HEADERS = ultimarc.h ulboard.h

