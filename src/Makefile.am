## Process this file with automake to product Makefile.in

dist_bin_SCRIPTS = sound_effects_editor

uidir = $(pkgdatadir)/ui
ui_DATA = sound_effects_editor.ui

EXTRA_DIST = $(ui_DATA)
EXTRA_DIST += sound_effects_editor.in

# Make sure the program knows where to find its files.
sound_effects_editor : sound_effects_editor.in
	sed -e 's%@pkgdatadir@%$(pkgdatadir)%g' $^ > $@

DISTCLEANFILES = sound_effects_editor
