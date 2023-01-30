# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: nkorkmaz <nkorkmaz@student.42.fr>          +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2022/12/07 10:28:14 by nkorkmaz          #+#    #+#              #
#    Updated: 2023/01/25 14:24:50 by nkorkmaz         ###   ########.fr        #
#                                                                              #
# **************************************************************************** #



NAME					= libftprintf.a

CC                      = gcc

SRCS					= ft_printf.c ft_process.c

OBJS					= $(SRCS:.c=.o)

FLAGS					= -Wall -Wextra -Werror

all	:	$(NAME)

$(NAME):	$(OBJS)
				$(CC) $(FLAGS) -c $(SRCS) -I./
				ar rc $(NAME) $(OBJS)

clean:
		rm -f $(OBJS)

fclean:	clean
		rm -f $(NAME)

re:	fclean all

.PHONY:	all clean fclean re