AM_CPPFLAGS =        \
  $(GLIB_CFLAGS)     \
  -I$(top_srcdir)/src \
  -I$(top_srcdir)/src/public

AM_CFLAGS = -Wall 
AM_CFLAGS += -Werror
# AM_CFLAGS += -Wpedantic

if ENABLE_CALLGRAPH_COND
AM_CFLAGS += -fdump-rtl-expand
endif


CLEANFILES = \
*expand

clean-local:
	@echo "(src/base/Makefile) clean-local"

mostlyclean-local:
	@echo "(src/base/Makefile) mostlyclean-local"

distclean-local:
	@echo "(src/base/Makefile) distclean-local"

dist-hook:
	@echo "(src/base/Makefile) dist-hook"

# Intermediate Library
noinst_LTLIBRARIES = libbase.la

libbase_la_SOURCES =      \
base_init.c               \
build_info.c              \
core.c                    \
ddc_errno.c               \
ddc_packets.c             \
dynamic_features.c        \
displays.c                \
execution_stats.c         \
feature_lists.c           \
feature_metadata.c        \
feature_sets.c            \
last_io_event.c           \
linux_errno.c             \
monitor_model_key.c       \
rtti.c                    \
sleep.c                   \
tuned_sleep.c             \
status_code_mgt.c         \
vcp_version.c


