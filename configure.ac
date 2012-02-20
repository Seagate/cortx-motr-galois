AC_PREREQ([2.59])
AC_INIT([galois], [0.1], [colibri@xyratex.com])
AC_CONFIG_SRCDIR([src/galois.c])
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

SRCDIR=$(cd $srcdir && echo $PWD)
if ! test -d $SRCDIR; then
	AC_MSG_ERROR([Cannot figure out full path for srcdir!])
fi
AC_SUBST([SRCDIR])

AC_MSG_CHECKING([for linux objects dir])
AC_ARG_WITH([linux-obj],
        [AC_HELP_STRING([--with-linux-obj=path],
                        [set path to Linux objects dir (default=/lib/modules/$(uname -r)/build])],
        [LINUX_OBJ=$with_linux_obj],
        [LINUX_OBJ=/lib/modules/$(uname -r)/build]
)

AC_MSG_RESULT([$LINUX_OBJ])
AC_SUBST([LINUX_OBJ])

LINUX_MOD=$(dirname $LINUX_OBJ)
AC_SUBST([LINUX_MOD])

AC_CONFIG_FILES([Makefile])
AC_CONFIG_FILES([doc/Makefile])
AC_CONFIG_FILES([src/Makefile])
AC_CONFIG_FILES([src/linux_kernel/Makefile])
AC_CONFIG_FILES([include/Makefile])
AC_CONFIG_FILES([include/galois/Makefile])
AC_CONFIG_FILES([galois.spec])
AC_OUTPUT
