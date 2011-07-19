AC_PREREQ([2.59])
AC_INIT([galois], [0.1], [colibri@xyratex.com])
AC_CONFIG_SRCDIR([galois.c])
AC_CONFIG_HEADERS([config.h])
AM_INIT_AUTOMAKE([galois],[0.1])
AC_CONFIG_MACRO_DIR([m4])
# Checks for programs.
AC_PROG_CC

AC_PROG_LIBTOOL

# Checks for header files.
AC_CHECK_HEADERS([stdlib.h string.h sys/time.h])

# Checks for typedefs, structures, and compiler characteristics.

# Checks for library functions.
AC_FUNC_MALLOC
AC_CHECK_FUNCS([gettimeofday])

AC_CONFIG_FILES([Makefile])
AC_CONFIG_FILES([doc/Makefile])
AC_OUTPUT
