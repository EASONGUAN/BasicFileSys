all: ext2_cp ext2_mkdir ext2_ln ext2_rm ext2_restore ext2_checker

ext2_cp: ext2_cp.o
	gcc -Wall -g -o $@ $^

ext2_mkdir: ext2_mkdir.o
	gcc -Wall -g -o $@ $^

ext2_ln: ext2_ln.o
	gcc -Wall -g -o $@ $^

ext2_rm: ext2_rm.o
	gcc -Wall -g -o $@ $^

ext2_restore: ext2_restore.o
	gcc -Wall -g -o $@ $^

ext2_checker: ext2_checker.o
	gcc -Wall -g -o $@ $^

%.o : %.c ext2.h
	gcc -Wall -g -c $<

clean :
	rm -f *.o ext2_cp ext2_mkdir ext2_ln ext2_rm ext2_restore ext2_checker *~
