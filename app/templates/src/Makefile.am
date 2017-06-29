if DEBUG
  AM_CFLAGS =-I$(top_srcdir)/src/lib -Wall -g -O3
else
  AM_CFLAGS =-I$(top_srcdir)/src/lib -Wall
endif

# Our binary is produced here
bin_PROGRAMS = <%= name %>
<%= name %>_SOURCES = main.c

# main binary will be installed into the default directory for "bin"s (hence we used the bin
# prefix
noinst_LIBRARIES = libhelper.a
libhelper_a_SOURCES = helper.c

# noinst_ : assures that this library is not installed to the user's computer
# libBLAH.a is a Unix convention. If you noticed, we replaced the . with _ in SOURCES line.
<%= generatorModuleNameWithUnderscores %>_LDADD = libhelper.a ../my_inc/libmyadd.a

# LDADD specifies which libraries to compile into "<%= generatorModuleNameWithUnderscores %>". We have two libraries.
# libhelper comes from this directory and libmyadd come from my_inc directory.
