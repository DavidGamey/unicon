TARGETS=$(patsubst %.icn,%.u,$(wildcard *.icn))

IC=../../bin/icont
UFLAGS= -usc

all:$(TARGETS)
	@cp *.u ../lib/

%.u: %.icn
	@echo $<
	@LPATH="../incl ../gincl ../mincl" $(IC) $(UFLAGS) $<

clean Clean:
	rm -f *.u
