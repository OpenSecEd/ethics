# $Id$

DOCUMENTS=	tracking.pdf
FILES=		tracking.tex aims.tex literature.tex literature.bib
CATEGORY=	security/seminars
PACKAGE=	tracking-src
TARBALL_FILES=	${FILES} Makefile
PUB_FILES=	${DOCUMENTS} ${PACKAGE}.tar.gz

tracking.pdf: ${FILES}

#export no

Makefile.export: Makefile
PACKAGE_FILES=	${FILES:.tex=.exporttex} Makefile.export

literature.bib: ../../infosak.bib
	${CP} $^ $@

clean:
	${RM} literature.bib

#endexport

### INCLUDES ###

miun.depend.mk:
	wget http://ver.miun.se/build/$@

include miun.depend.mk
include miun.course.mk
include miun.package.mk
include miun.export.mk
