# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: datran <datran@student.42.fr>              +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2022/11/14 12:12:32 by datran            #+#    #+#              #
#    Updated: 2022/12/18 14:20:50 by datran           ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

NAME		=	libft.a

SRCS		=	ft_atoi.c \
				ft_bzero.c \
				ft_calloc.c \
				ft_isalnum.c \
				ft_isalpha.c \
				ft_isascii.c \
				ft_isdigit.c \
				ft_isprint.c \
				ft_itoa.c \
				ft_itoa_base.c \
				ft_memcpy.c \
				ft_memchr.c \
				ft_memcmp.c \
				ft_memcpy.c \
				ft_memmove.c \
				ft_memset.c \
				ft_putchar_fd.c \
				ft_putendl_fd.c \
				ft_putnbr_fd.c \
				ft_putstr_fd.c \
				ft_split.c \
				ft_strchr.c \
				ft_strdup.c \
				ft_striteri.c \
				ft_strjoin.c \
				ft_strlcat.c \
				ft_strlcpy.c \
				ft_strlen.c \
				ft_strmapi.c \
				ft_strncmp.c \
				ft_strnstr.c \
				ft_strrchr.c \
				ft_strtrim.c \
				ft_substr.c \
				ft_tolower.c \
				ft_toupper.c

BNS_SRCS	=	ft_lstsize.c \
				ft_lstadd_back.c \
				ft_lstadd_front.c \
				ft_lstclear.c \
				ft_lstdelone.c \
				ft_lstiter.c \
				ft_lstlast.c \
				ft_lstmap.c \
				ft_lstnew.c

OBJS		=	$(SRCS:%.c=%.o)

BNS_OBJS	=	$(BNS_SRCS:%.c=%.o)

FLAGS		=	-Wall -Wextra -Werror

DEPS		=	-I./

$(NAME)		:	$(OBJS)
			gcc $(FLAGS) -c $(SRCS) $(DEPS)
			ar rc $(NAME) $(OBJS)

all			:	$(NAME)

bonus		:	$(NAME)
			gcc $(FLAGS) -c $(BNS_SRCS) $(DEPS)
			ar rc $(NAME) $(BNS_OBJS)

clean		:
			rm -f $(OBJS) $(BNS_OBJS)

fclean		:	clean
			rm -f $(NAME)

re			:	fclean all

.PHONY 		: all bonus clean fclean re
