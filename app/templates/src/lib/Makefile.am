if DEBUG
  AM_CFLAGS =-I$(top_srcdir)/src/lib -Wall -g -O3
else
  AM_CFLAGS =-I$(top_srcdir)/src/lib -Wall
endif


# The libraries to build
noinst_LIBRARIES = libcplain.a

# The files to add to the library and to the source distribution
libcplain_a_SOURCES = \
										     $(libcplain_a_HEADERS) \
										     cplain.c
