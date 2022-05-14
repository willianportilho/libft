<h1 align="center"> Libft </h1>

<p align="center"> A 42 project written in C language</p>

---

## introduction

<p> This project had the purpose of recode the usual C funtions for use in the future 42 projects. </p>

- [part_1](#part_1) - Set of recoded libc functions
- [part_2](#part_2) - Set of non-libc functions
- [bonus](#bonus) - Set of linked list funtions

## part_1
#### ctype.h lib
-> [`ft_isalnum`](/ft_isalnum.c) - Checks for an alphanumeric character.  
-> [`ft_isalpha`](/ft_isalpha.c) - Checks for an alphabetic character.  
-> [`ft_isascii`](/ft_isascii.c) - Checks whether c is a 7-bit unsigned char value that fits into the ASCII character set.  
-> [`ft_isdigit`](/ft_isdigit.c) - Checks for a digit (0 through 9).  
-> [`ft_isprint`](/ft_isprint.c) - Checks for any printable character including space.  
-> [`ft_tolower`](/ft_tolower.c) - Converts the letter c to lower case, if possible.  
-> [`ft_toupper`](/ft_toupper.c) - Converts the letter c to upper case, if possible.  
#### string.h lib
-> [`ft_bzero`](/ft_bzero.c) --- Erases the data in the n bytes of the memory starting at the location pointed to by s, by writing zeros ('\0').  
-> [`ft_memchr`](/ft_memchr.c) -- Scans the initial n bytes of the memory area pointed to by s for the first instance of c.  
-> [`ft_memcmp`](/ft_memcmp.c) -- Compares the first n bytes (each interpreted as unsigned char) of the memory areas s1 and s2.  
-> [`ft_memcpy`](/ft_memcpy.c) -- Copies n bytes from memory area src to memory area dest. The memory areas must not overlap.  
-> [`ft_memmove`](/ft_memmove.c) - Copies n bytes from memory area src to memory area dest. The memory areas may overlap.  
-> [`ft_memset`](/ft_memset.c) -- Fills the first n bytes of the memory area pointed to by s with the constant byte c.  
-> [`ft_strchr`](/ft_strchr.c) -- Returns a pointer to the first occurrence of the character c in the string s.  
-> [`ft_strdup`](/ft_strdup.c) -- Allocates and returns a pointer to a new string which is a duplicate of the string s.  
-> [`ft_strlen`](/ft_strlen.c) -- Calculates the length of the string pointed to by s, excluding the terminating null byte ('\0').  
-> [`ft_strncmp`](/ft_strncmp.c) - Compares n bytes of strings s1 and s2. (bytes that follow a '\0' character are not compared).  
-> [`ft_strnstr`](/ft_strnstr.c) - Finds and returns a pointer to the the first substring in a length-limited string.  
-> [`ft_strrchr`](/ft_strrchr.c) - Returns a pointer to the last occurrence of the character c in the string s.  
#### bsd/string.h lib
-> [`ft_strlcat`](/ft_strlcat.c) - Appends the NUL-terminated string src to the end of dst. It will append at most size - dst - 1 bytes, NUL-terminating the result.  
-> [`ft_strlcpy`](/ft_strlcpy.c) - Copies up to size - 1 characters from the NUL-terminated string src to dst, NUL-terminating the result.  
#### stdlib.h lib
-> [`ft_atoi`](/ft_atoi.c) ---- Converts the initial portion of the string pointed to by nptr to int.  
-> [`ft_calloc`](/ft_calloc.c) -- Allocates memory for an array of nmemb elements of size bytes each and returns a pointer to the allocated memory.  

## part_2
#### string functions
-> [`ft_split`](/ft_split.c) ----- Allocates and returns an array of strings obtained by splitting ’s’ using the character ’c’ as a delimiter.  
-> [`ft_substr`](/ft_substr.c) ---- Allocates and returns a substring from the string ’s’.  
-> [`ft_strjoin`](/ft_strjoin.c) --- Allocates and returns a new string, which is the result of the concatenation of ’s1’ and ’s2’.  
-> [`ft_strtrim`](/ft_strtrim.c) --- Allocates and returns a copy of ’s1’ with the characters specified in ’set’ removed from the beginning and the end of the string.  
-> [`ft_strmapi`](/ft_strmapi.c) --- Applies the function ’f’ to each character of the string ’s’, passing its index as first argument to create a new string.  
-> [`ft_striteri`](/ft_striteri.c) -- Applies the function ’f’ on each character of the string ’s’, passing its index as first argument to be modified if necessary.  
#### int to ascii function
-> [`ft_itoa`](/ft_itoa.c) ------- Allocates and returns a string representing the integer received as an argument.  
#### file descriptor (fd) functions
-> [`ft_putnbr_fd`](/ft_putnbr_fd.c) -- Outputs the integer ’n’ to the given file descriptor.  
-> [`ft_putstr_fd`](/ft_putstr_fd.c) -- Outputs the string ’s’ to the given file descriptor.  
-> [`ft_putchar_fd`](/ft_putchar_fd.c) - Outputs the character ’c’ to the given file descriptor.  
-> [`ft_putendl_fd`](/ft_putendl_fd.c) - Outputs the string ’s’ to the given file descriptor followed by a newline.  

## bonus
#### linked list functions
-> [`ft_lstmap`](/ft_lstmap.c) -------- Iterates the ’lst’ list and applies the function ’f’ (and ’del’ function if needed), on the content of each node. Creates a new list resulting of the successive applications of the function ’f’.  
-> [`ft_lstnew`](/ft_lstnew.c) -------- Allocates and returns a new node. The member variable ’content’ is initialized with the value of the parameter ’content’.  
-> [`ft_lstiter`](/ft_lstiter.c) ------- Iterates the list ’lst’ and applies the function ’f’ on the content of each node.  
-> [`ft_lstsize`](/ft_lstsize.c) ------- Counts the number of nodes in a list.  
-> [`ft_lstlast`](/ft_lstlast.c) ------- Returns the last node of the list.  
-> [`ft_lstclear`](/ft_lstclear.c) ------ Deletes and frees the given node and every successor of that node, using the function ’del’ given as a parameter.  
-> [`ft_lstdelone`](/ft_lstdelone.c) ----- Frees the memory of the node’s 'content' using the function ’del’ given as a parameter and free the node.  
-> [`ft_lstadd_back`](/ft_lstadd_back.c) -- Adds the node ’new’ at the end of the list.  
-> [`ft_lstadd_front`](/ft_lstadd_front.c) - Adds the node ’new’ at the beginning of the list.  
