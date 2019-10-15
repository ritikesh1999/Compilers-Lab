parser.out :	asgn4_17CS30027.c lex.yy.c y.tab.c
	gcc asgn4_17CS30027.c -lfl -I.  -o ./parser.out

y.tab.c : asgn4_17CS30027.y
	bison asgn4_17CS30027.y -o 'y.tab.c'

lex.yy.c : asgn4_17CS30027.l
	flex asgn4_17CS30027.l

clean: 
	rm -f ./*~ ./lex.yy.c ./y.tab.c ./parser.out

run: parser.out
	./parser.out < asgn4_17CS30027_test.c
