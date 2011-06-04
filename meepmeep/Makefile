# keyword: meepmeep
# puzzle: http://www.facebook.com/careers/puzzles.php?puzzle_id=3
# language: GNU C++ (gcc 4.2.1)
# build tool: GNU Make 3.81
# location: https://github.com/whittle/fb-puzzles-cpp
# author: Jason Whittle <jason.whittle@gmail.com>

CC = g++
CFLAGS = -g -Wall
RM = /bin/rm -f
TAR = /usr/bin/tar

PUZZLE = meepmeep

all: ${PUZZLE}

${PUZZLE}: src/${PUZZLE}.cpp
	${CC} ${CFLAGS} -o ${PUZZLE} src/${PUZZLE}.cpp

clean:
	${RM} ${PUZZLE}
	${RM} -r ${PUZZLE}.dSYM
	${RM} ${PUZZLE}.tgz

zip:
	${TAR} czf ${PUZZLE}.tgz Makefile src
