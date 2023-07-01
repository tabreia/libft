# 42cursus-libft ([Subject](/.github/en.subject.pdf))

## Description
This project is your very first project as a student at 42. You will need to recode a few functions of the C standard library as well as some other utility functions that you will use during your whole cursus.

## Usage

- Download the latest release.
- Include the libft header file in the project's header file or in the project's source files independently.
- Compile the project with the provided static library file (.a).

## Libft Reference

| Function          | Arguments         | Return Value                                                                     | Description                           |
| :---------------- | :---------------- | :------------------------------------------------------------------------------- | :------------------------------------ |
| `ft_isalpha`      | `unsigned char c` | nonzero if the character c falls into the tested class, and a zero value if not. | checks for an alphabetic character.   |
| `ft_isdigit`      | `unsigned char c` | nonzero if the character c falls into the tested class, and a zero value if not. | checks for a digit (0 through 9).     |
| `ft_isalnum`      | `unsigned char c` | nonzero if the character c falls into the tested class, and a zero value if not. | checks for an alphanumeric character. |
| `ft_isascii`      | `unsigned char c` | nonzero if the character c falls into the tested class, and a zero value if not. | checks whether c is a 7-bit unsigned char value that fits into the ASCII character set. |
| `ft_isprint`      | `unsigned char c` | nonzero if the character c falls into the tested class, and a zero value if not. | checks for any printable character including space. |
| `ft_strlen`       | `const char c`    | the number of bytes in the string s. | calculates the length of the string s, excluding the terminating null byte. |
| `ft_memset`       | `void *s` `int c` `size_t n` | returns a pointer to the memory area s. | fills the first n bytes of the memory area pointed to by s with the constant byte c. |
| `ft_bzero`        | `void *s` `size_t n` | none. | sets the first n bytes of the area starting at s to zero. |
| `ft_memcpy`       | `void *dest` `const void *src` `size_t n` | a pointer to dest. | copies n bytes from memory area src to memory area dest. The memory areas must not overlap. |
| `ft_memmove`      | `void *dest` `const void *src` `size_t n` | a pointer to dest. | copies n bytes from memory area src to memory area dest. |
| `ft_memchr`       | `void *dest` `const void *src` `size_t n` | a pointer to the matching byte or NULL if the character does not occur in the given memory area. | scans the initial n bytes of the memory area pointed to by s for the first instance of c. |
| `ft_memcmp`       | `void *s1` `void *s2` `size_t n` | an integer less than, equal to, or greater than zero if the first n bytes of s1 is found, respectively, to be less than, to match, or be greater than the first n bytes of s2. | compares the first n bytes (each interpreted as unsigned char) of the memory areas s1 and s2. |
| `ft_strchr`       | `const char *s` `int c` | a pointer to the matched character or NULL if the character is not found. | returns a pointer to the first occurrence of the character c in the string s. |
| `ft_strrchr`      | `const char *s` `int c` | a pointer to the matched character or NULL if the character is not found. | returns a pointer to the last occurrence of the character c in the string s. |
| `ft_strncmp`      | `const char *s1` `const char *s2` | an integer less than, equal to, or greater than zero if s1 (or the first n bytes thereof) is found, respectively, to be less than, to match, or be greater than s2. |  compares the two strings s1 and s2. |
| `ft_strlcpy`      | `char *dest` `const char *src` `size_t size` | the total length of the string they tried to create. | copies up to size - 1 characters from the NUL-terminated string src to dst, NUL-terminating the result. |
| `ft_strlcat`      | `char *dest` `const char *src` `size_t size` | the total length of the string they tried to create. | appends the NUL-terminated string src to the end of dst. It will append at most size - strlen(dst) - 1 bytes, NUL-terminating the result. |
| `ft_strstr`       | `const char *haystack` `const char *needle` | a pointer to the beginning of the substring, or NULL if the substring is not found. | finds the first occurrence of the substring needle in the string haystack. |
| `ft_atoi`         | `const char *nptr` | the converted value. | converts the initial portion of the string pointed to by nptr to int. |
| `ft_toupper`      | `int c` | the converted letter, or c if the conversion was not possible. | converts the letter c to upper case, if possible. |
| `ft_tolower`      | `int c` | the converted letter, or c if the conversion was not possible. | converts the letter c to lower case, if possible. |
| `ft_calloc`       | `size_t size` | a pointer to the allocated memory that is suitably aligned for any kind of variable. On error, these functions return NULL. | allocates memory for an array of nmemb elements of size bytes each and returns a pointer to the allocated memory. The memory is set to zero. |
| `ft_strdup`       | `const char *s` | a pointer to the duplicated string, or NULL if insufficient memory was available. | allocates and returns a pointer to a new string which is a duplicate of the string s. |
| `ft_substr`       | `const char *s` `unsigned int start` `size_t len` | the substring, or NULL if the allocation fails. | allocates and returns a substring from the string ’s’. The substring begins at index ’start’ and is of maximum size ’len’. |
| `ft_strjoin`      | `const char *s1` `const char *s2` | the new string, or NULL if the allocation fails. | allocates and returns a new string, which is the result of the concatenation of ’s1’ and ’s2’. |
| `ft_strtrim`      | `const char *s1` `const char *set` | the trimmed string, or NULL if the allocation fails. | allocates and returns a copy of ’s1’ with the characters specified in ’set’ removed from the beginning and the end of the string. |
| `ft_split`        | `const char *s` `char c` | the array of new strings resulting from the split, or NULL if the allocation fails. | allocates and returns an array of strings obtained by splitting ’s’ using the character ’c’ as a delimiter. The array must end with a NULL pointer. |
| `ft_itoa`         | `int n` | the string representing the integer, or NULL if the allocation fails. | allocates and returns a string representing the integer received as an argument. |
| `ft_strmapi`      | `const char *s` `char (*f)(unsigned int, char)`| The string created from the successive applications of ’f’, or NULL if the allocation fails. | allocates and applies the function ’f’ to each character of the string ’s’, and passing its index as first argument to create a new string resulting from successive applications of ’f’. |
| `ft_striteri`     | `char *s` `void (*f)(unsigned int, char *)`| none. | applies the function ’f’ on each character of the string passed as argument, passing its index as first argument. Each character is passed by address to ’f’ to be modified if necessary. |
| `ft_putchar_fd`   | `char c` `int fd` | none. | outputs the character ’c’ to the given file descriptor. |
| `ft_putstr_fd`    | `char *s` `int fd` | none. | outputs the string ’s’ to the given file descriptor. |
| `ft_putendl_fd`   | `char *s` `int fd` | none. | outputs the string ’s’ to the given file descriptor followed by a new line. |
| `ft_putnbr_fd`    | `int n` `int fd` | none. | outputs the integer ’n’ to the given file descriptor. |
| `ft_lstnew`       | `void *content` | the new node. | allocates and returns a new node. The member variable ’content’ is initialized with the value of the parameter ’content’. The variable ’next’ is initialized to NULL. |
| `ft_lstadd_front` | `t_list **lst` `t_list *new` | none. | adds the node ’new’ at the beginning of the list. |
| `ft_lstsize`      | `t_list *lst` | the length of the list. | counts the number of nodes in a list. |
| `ft_lstlast`      | `t_list *lst` | last node of the list. | returns the last node of the list. |
| `ft_lstadd_back`  | `t_list **lst` `t_list *new` | none. | adds the node ’new’ at the end of the list. |
| `ft_lstdelone`    | `t_list *lst` `void (*del)(void *)` | none. | takes as a parameter a node and frees the memory of the node’s content using the function ’del’ given as a parameter and free the node. |
| `ft_lstclear`     | `t_list *lst` `void (*del)(void *)` | none. | deletes and frees the given node and every successor of that node, using the function ’del’ and free(3). |
| `ft_lstiter`      | `t_list *lst` `void (*f)(void *)` | none. | iterates the list ’lst’ and applies the function ’f’ on the content of each node. |
| `ft_lstmap`       | `t_list *lst` `void *(*f)(void *)` `void (*del)(void *)` | The new list, or NULL if the allocation fails. | iterates the list ’lst’ and applies the function ’f’ on the content of each node. Creates a new list resulting of the successive applications of the function ’f’. The ’del’ function is used to delete the content of a node if needed. |

| Function          | Arguments  | Return Value                                                                     | Description                           |
| :---------------- | :--------- | :------------------------------------------------------------------------------- | :------------------------------------ |
| `get_next_line`   | `int fd`   | the read line, or NULL if there is nothing else to read, or an error occurred.   | write a function that returns a line read from a file descriptor.   |
| `ft_printf`       | `const char *format` | return the number of characters printed | produce output according to a format. only cspdiuxX% is available in this function. |
| `ft_fndnrepl`       | `const char *find_str` `char *replace_word` `char *replace_value` | the new string, or NULL if the allocation fails. | find and replace a 'replace_word' by a 'replace_value' within 'find_str' |

[![GitHub](https://img.shields.io/github/license/BrunoCostaGH/42cursus-libft?style=for-the-badge)](https://github.com/BrunoCostaGH/42cursus-libft)
[![GitHub contributors](https://img.shields.io/github/contributors/BrunoCostaGH/42cursus-libft?style=for-the-badge)](https://github.com/BrunoCostaGH/42cursus-libft)
[![GitHub issues](https://img.shields.io/github/issues/BrunoCostaGH/42cursus-libft?style=for-the-badge)](https://github.com/BrunoCostaGH/42cursus-libft/issues)
[![GitHub Release Date](https://img.shields.io/github/release-date/BrunoCostaGH/42cursus-libft?style=for-the-badge)](https://github.com/BrunoCostaGH/42cursus-libft/releases/latest)
[![GitHub release (latest by date)](https://img.shields.io/github/v/release/BrunoCostaGH/42cursus-libft?style=for-the-badge)](https://github.com/BrunoCostaGH/42cursus-libft/releases/latest)

[![FT_PRINTF](https://img.shields.io/badge/FT__PRINTF-v1.0.0-informational?style=for-the-badge)](https://github.com/BrunoCostaGH/42cursus-ft_printf/tree/v1.0.0)
