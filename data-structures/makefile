.PHONY :
	build

build : static clean_o

static : objects
	ar -crs libAllDS.a *o

objects :
	gcc -c -std=c89 -Wall -Werror -Wextra -Wshadow -pedantic-errors -O3 \
	linked-list/int-list.c queue/queue-by-list.c hash-table/external-chain.c \
	stack/stack-imp.c binary-tree/bin-tree.c binary-tree/btn-queue.c -I.

clean :
	rm liballds.a

clean_o :
	rm *.o
