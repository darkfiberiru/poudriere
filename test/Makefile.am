TESTS=\
	cache.sh \
	encode_args.sh \
	getvar.sh \
	gsub.sh \
	hash_basic.sh \
	list.sh \
	locks.sh \
	locks_critical_section.sh \
	locks_critical_section_nested.sh \
	mapfile.sh \
	port_var_fetch.sh \
	prefix_output.sh \
	read_file.sh \
	relpath.sh \
	relpath_common.sh \
	shash_basic.sh \
	trap_save.sh \
	bulk-bad-DEPENDS_ARGS.sh \
	bulk-ignore-listed.sh \
	bulk-ignore-dep-skipped.sh \
	bulk-ignore-listed-skipped-dep.sh \
	bulk-ignore-listed-dep.sh \
	bulk-ignore-and-skipped.sh \
	bulk-flavor-default-dep-and-specific-listed.sh \
	bulk-flavor-default-dep.sh \
	bulk-flavor-main-dep-and-default-listed.sh \
	bulk-flavor-main-dep-and-specific-listed.sh \
	bulk-flavor-main-dep.sh \
	bulk-flavor-nonexistent.sh \
	bulk-flavor-specific-dep-and-default-listed.sh \
	bulk-flavor-specific-dep-and-default-shorthand-listed.sh \
	bulk-flavor-specific-dep-and-main-listed_default_all_off.sh \
	bulk-flavor-specific-dep-and-main-listed_default_all_off_w_@all.sh \
	bulk-flavor-specific-dep-and-main-listed_default_all_on.sh \
	bulk-flavor-specific-dep-and-multi-listed.sh \
	bulk-flavor-specific-dep-and-multi-no-main-listed.sh \
	bulk-flavor-specific-dep-and-specific-listed.sh \
	bulk-flavor-specific-dep-and-specific-listed-nonexistent.sh \
	bulk-flavor-specific-dep-nonexistent.sh \
	bulk-flavor-specific-dep.sh \
	bulk-flavor-metadata-queue-ordering.sh \
	bulk-flavor-metadata-queue-ordering-multi-pass.sh \
	bulk-flavor-ignore-all.sh \
	bulk-overlay-all.sh \
	bulk-no-overlay-specific.sh \
	bulk-overlay-specific.sh

run_env=	env PATH="$(abs_top_builddir):$$PATH" VPATH=$(VPATH)
LOG_COMPILER=	$(run_env) ${SH} $(srcdir)/runtest.sh
#TEST_EXTENSIONS=.sh
#SH_LOG_COMPILER=$(run_env) ${SH} runtest.sh

check-am: prep

.PHONY: prep
prep:
	@echo "Prepping test jail"
	@cd $(srcdir) && $(run_env) ${SH} prep.sh
