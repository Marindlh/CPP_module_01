# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: madelaha <marvin@42.fr>                    +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2022/11/01 17:24:01 by madelaha          #+#    #+#              #
#    Updated: 2022/11/03 13:46:32 by madelaha         ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

NAME = zombie

HEADER = Zombie.hpp

SRCS = Zombie.cpp \
	   newZombie.cpp \
	   randomChump.cpp \
	   main.cpp \

OBJS = ${SRCS:.cpp=.o}

RM = rm -f

CFLAGS = -Wall -Wextra -Werror -std=c++98

CC = c++ ${CFLAGS}

.cpp.o:
		${CC} -c $< -o ${<:.cpp=.o}

${NAME}:	${OBJS}
			${CC} ${OBJS} -o ${NAME}

all: ${NAME}

clean:
		${RM} ${OBJS}

fclean: clean
		${RM} ${OBJS}

re: fclean all

.PHONY: all clean fclean re
