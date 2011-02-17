#!/usr/bin/make

PDFNAME=pvete10_slides_lprog10

SRC=src/
OBJ=obj/

MAINNAME=main
RUBBERFLAGS=-d --into $(OBJ) -I.

all:
	@echo [RUBBER] $(SRC)$(MAINNAME)
	@rubber $(RUBBERFLAGS) $(SRC)$(MAINNAME)

	@echo -n "[MV] "
	@mv -v $(OBJ)$(MAINNAME).pdf $(PDFNAME).pdf

clean:
	@echo [RUBBER] clean
	@rubber $(RUBBERFLAGS) --clean $(SRC)$(MAINNAME)

mrproper: clean
	@echo -n "[RM] "
	@rm -vf $(PDFNAME).pdf

.PHONY: clean mrproper
