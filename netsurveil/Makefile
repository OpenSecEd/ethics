DOCUMENTS=	netsurveil.pdf
FILES=		netsurveil.tex aims.tex literature.tex literature.bib
CATEGORY=	security/seminars

PACKAGE= 		netsurveil-src
TARBALL_FILES= 	${FILES} Makefile

USE_BIBLATEX= 	yes
USE_LATEXMK= 	yes

netsurveil.pdf: ${FILES}

#export no
PUB_FILES= 		${DOCUMENTS} ${PACKAGE}.tar.gz

literature.bib: ../../infosak.bib
	${CP} $^ $@

clean:
	${RM} literature.bib ${DOCUMENTS}
#endexport

miun.depend.mk:
	wget http://ver.miun.se/build/$@

include miun.depend.mk
include miun.course.mk
include miun.package.mk
