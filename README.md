# Multibyte String Manipulation Library

This library provides a set of functions for manipulating multibyte strings in C. It includes functions for calculating string lengths, comparing strings, copying and concatenating strings, and searching for characters within strings.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Functions](#functions)
- [License](#license)

## Installation
1. git clone https://github.com/kaan-yalcinkaya/MBString
2. cd MBString
3. cmake -B build -D CMAKE_BUILD_TYPE=Release
4. cmake --build build

## Usage
Include the multibyte_string.h header file in your source code:<br>
```#include "multibyte_string.h"```<br>
You can then use the provided functions to manipulate multibyte strings in your application.

## Functions
size_t mbslen(const char* mbs)<br>
Calculates the length of a multibyte string.<br>

size_t mbsnlen(const char* mbs, size_t n)<br>
Calculates the length of a multibyte string up to a specified limit.<br>

int mbsncmp(char* mbs1, char* mbs2, size_t n)<br>
Compares two multibyte strings up to a specified number of characters.<br>

char* mbsncpy(char* dest, size_t cbDest, const char* src, size_t n)<br>
Copies up to a specified number of characters from one multibyte string to another.<br>

char* mbsncat(char* dest, size_t cbDest, const char* src, size_t n)<br>
Concatenates up to a specified number of characters from one multibyte string to another.<br>

char* mbschr16(char* mbs, char16_t c)<br>
Locates the first occurrence of a 16-bit character in a multibyte string.<br>

char* mbschr32(char* mbs, char32_t c)<br>
Locates the first occurrence of a 32-bit character in a multibyte string.<br>

char* mbsrchr16(char* mbs, char16_t c)<br>
Locates the last occurrence of a 16-bit character in a multibyte string.<br>

char* mbsrchr32(char* mbs, char32_t c)<br>
Locates the last occurrence of a 32-bit character in a multibyte string.<br>

char* mbspbrk(char* mbs1, char* mbs2)<br>
Locates the first occurrence in a multibyte string of any of the characters in another string.<br>

size_t mbsspn(char* mbs1, char* mbs2)<br>
Calculates the length of the initial segment of a multibyte string consisting of characters not in another string.<br>
