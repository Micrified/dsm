CC=gcc
CFLAGS= -Wall -Wextra -D_GNU_SOURCE
LIBS=-ldsm -lpthread -lrt -lxed

# BUILD RULES

all: pingpong_busy_wait pingpong_semaphore dsm_pi

pingpong_busy_wait: pingpong_busy_wait.c
	${CC} ${CFLAGS} -o pingpong_busy_wait pingpong_busy_wait.c ${LIBS}

pingpong_semaphore: pingpong_semaphore.c
	${CC} ${CFLAGS} -o pingpong_semaphore pingpong_semaphore.c ${LIBS}

dsm_pi: dsm_pi.c
	${CC} ${CFLAGS} -o dsm_pi dsm_pi.c ${LIBS}


# CLEAN RULES

clean:
	rm pingpong_busy_wait
	rm pingpong_semaphore
	rm dsm_pi
