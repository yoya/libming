SUBDIRS = 

AM_CPPFLAGS = \
	-I$(top_srcdir) \
	-I$(top_srcdir)/src \
	-I$(top_srcdir)/test

LDADD = $(top_builddir)/src/libming.la

TESTS = dotests

C_PROGS =		\
	test01		
if USE_CXX
CXX_PROGS =		\
	test01-cxx	

test01_cxx_SOURCES = test01-cxx.C
endif

TEST_PROGS = $(C_PROGS) $(CXX_PROGS)

EXTRA_DIST = 		\
	test01.ref	\
	test01.pl	\
	test01.php	\
	TestList

check_PROGRAMS = \
	$(TEST_PROGS)

test01_SOURCES = test01.c

CLEANFILES = dotests test01.swf php.ini

include ../../Makefile.inc
