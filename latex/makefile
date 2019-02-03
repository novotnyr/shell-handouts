shell-business-cards.pdf: shell-business-cards.tex
	xelatex shell-business-cards.tex
shell-business-cards-nup.pdf: shell-business-cards.pdf
	pdfjam --suffix nup --nup '2x5' --frame true --noautoscale true -- shell-business-cards.pdf
	
