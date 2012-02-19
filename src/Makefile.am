SUBDIRS                  = linux_kernel

lib_LTLIBRARIES          = libgalois.la
noinst_PROGRAMS          = gf_basic_tester gf_div gf_ilog gf_inverse gf_log gf_mult gf_xor gf_xor_tester

libgalois_la_SOURCES     = galois.c
libgalois_la_INCLUDES    = -I$(top_srcdir) -I$(top_srcdir)/include
libgalois_la_LDFLAGS     = -release 0.1

gf_basic_tester_SOURCES  = gf_basic_tester.c
gf_basic_tester_INCLUDES = -I$(top_srcdir) -I$(top_srcdir)/include
gf_basic_tester_LDADD    = $(top_builddir)/src/libgalois.la

gf_div_SOURCES           = gf_div.c
gf_div_INCLUDES          = -I$(top_srcdir) -I$(top_srcdir)/include
gf_div_LDADD             = $(top_builddir)/src/libgalois.la

gf_ilog_SOURCES          = gf_ilog.c
gf_ilog_INCLUDES         = -I$(top_srcdir) -I$(top_srcdir)/include
gf_ilog_LDADD            = $(top_builddir)/src/libgalois.la

gf_inverse_SOURCES       = gf_inverse.c
gf_inverse_INCLUDES      = -I$(top_srcdir) -I$(top_srcdir)/include
gf_inverse_LDADD         = $(top_builddir)/src/libgalois.la

gf_log_SOURCES           = gf_log.c
gf_log_INCLUDES          = -I$(top_srcdir) -I$(top_srcdir)/include
gf_log_LDADD             = $(top_builddir)/src/libgalois.la

gf_mult_SOURCES          = gf_mult.c
gf_mult_INCLUDES         = -I$(top_srcdir) -I$(top_srcdir)/include
gf_mult_LDADD            = $(top_builddir)/src/libgalois.la

gf_xor_SOURCES           = gf_xor.c
gf_xor_INCLUDES          = -I$(top_srcdir) -I$(top_srcdir)/include
gf_xor_LDADD             = $(top_builddir)/src/libgalois.la

gf_xor_tester_SOURCES    = gf_xor_tester.c
gf_xor_tester_INCLUDES   = -I$(top_srcdir) -I$(top_srcdir)/include
gf_xor_tester_LDADD      = $(top_builddir)/src/libgalois.la
