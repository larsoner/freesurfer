## 
## Makefile.am 
##

AM_CFLAGS=-I$(top_srcdir)/include -I$(top_srcdir)/include/dicom
AM_LDFLAGS=

bin_PROGRAMS = mri_matrix_multiply
mri_matrix_multiply_SOURCES=mri_matrix_multiply.c
mri_matrix_multiply_LDADD= $(addprefix $(top_builddir)/, $(LIBS_MGH))
mri_matrix_multiply_LDFLAGS=$(OS_LDFLAGS)

TESTS=test.py

EXTRA_DIST= test.py

# Our release target. Include files to be excluded here. They will be
# found and removed after 'make install' is run during the 'make
# release' target.
EXCLUDE_FILES=""
include $(top_srcdir)/Makefile.extra
