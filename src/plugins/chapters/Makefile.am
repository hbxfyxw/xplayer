include $(top_srcdir)/src/plugins/Makefile.plugins

plugindir = $(PLUGINDIR)/chapters
plugin_LTLIBRARIES = libchapters.la

plugin_in_files = chapters.plugin.in

uidir = $(plugindir)
ui_DATA = chapters-list.ui chapters-edit.ui
EXTRA_DIST += $(ui_DATA)

libchapters_la_SOURCES = \
	xplayer-chapters.c	\
	xplayer-cmml-parser.c	\
	xplayer-cmml-parser.h	\
	xplayer-chapters-utils.c	\
	xplayer-chapters-utils.h	\
	xplayer-edit-chapter.c	\
	xplayer-edit-chapter.h
libchapters_la_LDFLAGS = $(plugin_ldflags)
libchapters_la_LIBADD = \
	$(plugin_libadd)	\
	$(CHAPTERS_LIBS)
libchapters_la_CFLAGS = \
	$(plugin_cflags)	\
	$(CHAPTERS_CFLAGS)

-include $(top_srcdir)/git.mk
