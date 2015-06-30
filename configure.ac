AC_INIT([samtools], [0.1.20], [gmarcais@umd.edu])
AC_CANONICAL_HOST
AC_CONFIG_MACRO_DIR([m4])
AM_INIT_AUTOMAKE([subdir-objects foreign parallel-tests color-tests])
AM_SILENT_RULES([yes])
AC_CONFIG_SRCDIR([.])
AC_CONFIG_HEADERS([config.h])

AC_PROG_LIBTOOL
AC_PROG_CC

# Check for curses
AC_SEARCH_LIBS([initscr], [ncurses curses], [CURSES_LIB=1], [CURSES_LIB=0])
AC_SUBST([CURSES_LIB])


AC_CONFIG_FILES([Makefile])
AC_OUTPUT
