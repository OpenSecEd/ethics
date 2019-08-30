.PHONY: all
all: instructions.pdf slides.pdf

SRC+=		preamble.tex security-society-seminar.bib
SRC+=		abstract.tex contents.tex

instructions.pdf: instructions.tex
instructions.pdf: ${SRC}

slides.pdf: slides.tex
slides.pdf: ${SRC}


.PHONY: clean
clean:
	${RM} instructions.pdf slides.pdf


INCLUDE_MAKEFILES=../makefiles
include ${INCLUDE_MAKEFILES}/tex.mk
