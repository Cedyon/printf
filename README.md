ALX Software Enginering Printf Team Project
This team project is a custom made printf function for the C programming language called _printf. It has been optimized to take various inputs and optional arguments based exactly on how the standard library function printf works. We submitted this as part of the ALX software engineering course requirement for grading.

Synopsis
This function _printf() writes output to stdout, the standard output stream with the format and options without making use of any of the standard library files. It was written to use a local buffer of 1024 bytes when printing although it can print larger sets of data.

The _printf() function returns the total number of characters printed to the stdout(excluding the null byte at the end of strings) after a successful execution.

If an output error is encountered, a negative value of -1 is returned.

The prototype of this function is: int _printf(const char format, ...);

This means that it has one mandatory format argument, and an extra number of arguments that can be none, or many.

Format of the format string

The format string is a character string starting and ending with double quotes. The format string is composed of zero or more directives; ordinary characters (not %), and conversion specifications, each of which results in fetching zero or more subsequent arguments.

Each conversion specification is introduced by the character % and ends with a conversion specifier. In between there may be (in this order):

Zero or more flags

An optional field width

An optional precision modifier

An optional length modifier

The flag characters


An optional decimal digit string (with nonzero first digit) specifying a minimum field width. If the converted value has fewer characters than the field width, it will be padded with spaces on the left if the flag - is not present, and on the right if it is present. A character * can be used instead of a decimal string. In this case, an argument passed to the function will be taken as the width value.

printf("%5d", num);
or

printf("%*d", width, num);
The precision

An optional precision, in the form of a period ('.') followed by an optional decimal digit string. A negative precision is taken as if the precision were omitted. This gives the minimum number of digits to appear for d, i, o, u, x, and X conversions, or the maximum number of characters to be printed from a string for s and S conversions. A character * can be 
Specifier	Description
d, i	The argument int is converted to a signed decimal notation. If precision is present,it gives the minimum number of digits that must appear; if the converted value requires fewer digits, then it is padded with zeros on the left. Default precision is 1.
o, u, x, X	The argument is converted to unsigned octal (o), unsigned decimal 
These instructions will get you a copy of the project up and running on your local machine (Linux distro) for development and testing purposes.

Installing
You will need to clone the repository of the project from Github. This will contain the _printf function and all of its dependencies. No main.c file will be provided for testing, so you will need to create one.

git clone https://github.com/Cedyon/printf.git
After cloning the repository you will have a folder called printf. In here there will be several files that allow the function to work.

Author: Cedrick Onyango 
Submitted by Cedrick Onyango and John Kagiri 
