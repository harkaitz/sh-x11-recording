PROJECT=sh-x11-recording
VERSION=1.0.0
PREFIX=/usr/local
all:
clean:
install:

## -- BLOCK:license --
install: install-license
install-license: 
	mkdir -p $(DESTDIR)$(PREFIX)/share/doc/$(PROJECT)
	cp LICENSE  $(DESTDIR)$(PREFIX)/share/doc/$(PROJECT)
## -- BLOCK:license --
## -- BLOCK:sh --
install: install-sh
install-sh:
	mkdir -p $(DESTDIR)$(PREFIX)/bin
	cp bin/xrec-start       $(DESTDIR)$(PREFIX)/bin
	cp bin/pulse-h          $(DESTDIR)$(PREFIX)/bin
	cp bin/xrec-menu        $(DESTDIR)$(PREFIX)/bin
	cp bin/dia-h-xpdf       $(DESTDIR)$(PREFIX)/bin
	cp bin/xrec-ffmpeg      $(DESTDIR)$(PREFIX)/bin
## -- BLOCK:sh --
