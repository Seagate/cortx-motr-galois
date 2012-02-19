SUBDIRS                  = . linux_kernel

lib_LTLIBRARIES          = libgalois.la
libgalois_la_SOURCES     = galois.c
libgalois_la_LDFLAGS     = -release 0.1

EXTRA_DIST 		 = gf_basic_tester.c gf_div.c gf_ilog.c gf_inverse.c \
                           gf_log.c gf_mult.c gf_xor.c gf_xor_tester.c

INCLUDES                  = -I$(top_srcdir) -I$(top_srcdir)/include

