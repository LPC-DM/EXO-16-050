TARGET = EXO-16-050_temp.pdf
all:	$(TARGET)

$(TARGET): $(wildcard *.tex) $(wildcard *.pdf)
	@cd ../../; ./tdr --style=pas b EXO-16-050

clean:
	@cd ../../; ./tdr clean

final: $(wildcard *.tex) $(wildcard figures/dataMC/*.pdf)
	@cd ../../; ./tdr --nodraft --style=pas b EXO-16-050
prl: $(wildcard *.tex) $(wildcard figures/dataMC/*.pdf)
	@cd ../../; ./tdr --nodraft --style=paper,aps,twocolumn b EXO-16-050/trunk/EXO-16-050
