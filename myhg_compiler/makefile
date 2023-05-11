c5c: lex.yy.c y.tab.c myhgc.c
	gcc -o myhgc.c lex.yy.c y.tab.c myhgc.c

lex.yy.c: myhg1.l
	flex myhg.l

y.tab.c: myhg.y
	bison -y -d myhg.y

nas:
	flex nas.l
	bison -d nas.y
	gcc -o nas lex.yy.c nas.tab.c
