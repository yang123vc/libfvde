AM_CPPFLAGS = \
	-I$(top_srcdir)/include \
	-I$(top_srcdir)/common \
	@LIBCERROR_CPPFLAGS@ \
	@LIBCDATA_CPPFLAGS@ \
	@LIBCLOCALE_CPPFLAGS@ \
	@LIBCNOTIFY_CPPFLAGS@ \
	@LIBCSPLIT_CPPFLAGS@ \
	@LIBUNA_CPPFLAGS@ \
	@LIBCFILE_CPPFLAGS@ \
	@LIBCPATH_CPPFLAGS@ \
	@LIBBFIO_CPPFLAGS@ \
	@LIBCSYSTEM_CPPFLAGS@ \
	@PTHREAD_CPPFLAGS@ \
	@LIBFVDE_DLL_IMPORT@

TESTS = \
	test_api_functions.sh \
	test_api_types.sh \
	test_fvdeinfo.sh

check_SCRIPTS = \
	test_api_functions.sh \
	test_api_types.sh \
	test_fvdeinfo.sh \
	test_runner.sh

EXTRA_DIST = \
	$(check_SCRIPTS)

check_PROGRAMS = \
	fvde_test_encryption_context_plist \
	fvde_test_error \
	fvde_test_logical_volume \
	fvde_test_notify \
	fvde_test_support \
	fvde_test_volume \
	fvde_test_volume_group

fvde_test_encryption_context_plist_SOURCES = \
	fvde_test_encryption_context_plist.c \
	fvde_test_libcerror.h \
	fvde_test_libfvde.h \
	fvde_test_macros.h \
	fvde_test_memory.c fvde_test_memory.h \
	fvde_test_unused.h

fvde_test_encryption_context_plist_LDADD = \
	../libfvde/libfvde.la \
	@LIBCERROR_LIBADD@

fvde_test_error_SOURCES = \
	fvde_test_error.c \
	fvde_test_libfvde.h \
	fvde_test_macros.h \
	fvde_test_unused.h

fvde_test_error_LDADD = \
	../libfvde/libfvde.la

fvde_test_notify_SOURCES = \
	fvde_test_libfvde.h \
	fvde_test_macros.h \
	fvde_test_notify.c \
	fvde_test_unused.h

fvde_test_notify_LDADD = \
	../libfvde/libfvde.la

fvde_test_logical_volume_SOURCES = \
	fvde_test_libcerror.h \
	fvde_test_libfvde.h \
	fvde_test_logical_volume.c \
	fvde_test_macros.h \
	fvde_test_memory.c fvde_test_memory.h \
	fvde_test_unused.h

fvde_test_logical_volume_LDADD = \
	../libfvde/libfvde.la \
	@LIBCERROR_LIBADD@

fvde_test_support_SOURCES = \
	fvde_test_libcerror.h \
	fvde_test_libclocale.h \
	fvde_test_libcsystem.h \
	fvde_test_libfvde.h \
	fvde_test_libuna.h \
	fvde_test_macros.h \
	fvde_test_support.c

fvde_test_support_LDADD = \
	@LIBCSYSTEM_LIBADD@ \
	@LIBUNA_LIBADD@ \
	@LIBCNOTIFY_LIBADD@ \
	@LIBCLOCALE_LIBADD@ \
	@LIBCDATA_LIBADD@ \
	../libfvde/libfvde.la \
	@LIBCERROR_LIBADD@

fvde_test_volume_SOURCES = \
	fvde_test_libcerror.h \
	fvde_test_libclocale.h \
	fvde_test_libcsystem.h \
	fvde_test_libfvde.h \
	fvde_test_libuna.h \
	fvde_test_macros.h \
	fvde_test_memory.c fvde_test_memory.h \
	fvde_test_volume.c

fvde_test_volume_LDADD = \
	@LIBCSYSTEM_LIBADD@ \
	@LIBUNA_LIBADD@ \
	@LIBCNOTIFY_LIBADD@ \
	@LIBCLOCALE_LIBADD@ \
	@LIBCDATA_LIBADD@ \
	../libfvde/libfvde.la \
	@LIBCTHREADS_LIBADD@ \
	@LIBCERROR_LIBADD@ \
	@PTHREAD_LIBADD@

fvde_test_volume_group_SOURCES = \
	fvde_test_libcerror.h \
	fvde_test_libfvde.h \
	fvde_test_macros.h \
	fvde_test_memory.c fvde_test_memory.h \
	fvde_test_unused.h \
	fvde_test_volume_group.c

fvde_test_volume_group_LDADD = \
	../libfvde/libfvde.la \
	@LIBCERROR_LIBADD@

MAINTAINERCLEANFILES = \
	Makefile.in

distclean: clean
	/bin/rm -f Makefile

