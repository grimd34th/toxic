bin_PROGRAMS = toxic


toxic_SOURCES = $(top_srcdir)/src/main.c \
                $(top_srcdir)/src/chat.h \
                $(top_srcdir)/src/chat.c \
                $(top_srcdir)/src/configdir.h \
                $(top_srcdir)/src/configdir.c \
                $(top_srcdir)/src/prompt.h \
                $(top_srcdir)/src/prompt.c \
                $(top_srcdir)/src/friendlist.h \
                $(top_srcdir)/src/friendlist.c \
                $(top_srcdir)/src/toxic_windows.h \
                $(top_srcdir)/src/windows.c \
                $(top_srcdir)/src/groupchat.c \
                $(top_srcdir)/src/groupchat.h \
                $(top_srcdir)/src/commands.c \
                $(top_srcdir)/src/commands.h \
                $(top_srcdir)/src/misc_tools.c \
                $(top_srcdir)/src/misc_tools.h

toxic_CFLAGS =	-I$(top_srcdir) \
				$(NCURSES_CFLAGS) \
				$(LIBSODIUM_CFLAGS) \
				$(LIBTOXCORE_CFLAGS)

toxic_CPPFLAGS = '-DTOXICVER="$(TOXIC_VERSION)"'

toxic_LDADD =	$(LIBTOXCORE_LDFLAGS) \
				$(LIBSODIUM_LDFLAGS) \
				$(NCURSES_LIBS) \
				$(LIBTOXCORE_LIBS) \
				$(LIBSODIUM_LIBS) \
                $(WINSOCK2_LIBS)

