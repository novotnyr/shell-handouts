shell-business-cards.pdf: shell-business-cards.tex
	xelatex $<
shell-business-cards-nup.pdf: shell-business-cards.pdf
	pdfjam --suffix nup --nup '2x5' --frame true --noautoscale true -- $<
nup: shell-business-cards-nup.pdf
.PHONY: nup	

all: shell-business-cards-nup.pdf shell-business-cards.pdf
	mv $^ ../docs
.PHONY: all

clean:
	rm *.aux *.log *.pdf
