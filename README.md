# JcopyS
the script copies the selected file to the specified directory a certain number of times

NAME
	JcopyS -- copying the selected file a certain number of times to a given directory.

SYNOPSIS
	JcopyS [-dhrs] [FILE] [PATH] [COUNT]

DESCRIPTION
	This script copies FILE along a given PATH a COUNT number of times.
	Each copy has the same name as original file + number of copy.

	-d
		Allows to copy a directory.

	-h, --help
		Show this help text.

	-r
		Will not show the CONFIRMATION for copy.
		(Not recommended for use.)

	-s
		Silent mode. Will not show any output messages except of flags error and CONFIRMATION{}.

	If input for PATH is missing, FILE will copy in present directory (.) a COUNT number of times.
	If input for COUNT is missing, FILE will copy along a PATH 1 time.
	IF input for PATH and COUNT is missing, FILE will copy in present directory (.) 1 time.

CONFIRMATION
	Before copying, the program will request confirmation of user execution in the specified format:
	'Are you sure you want to copy FILE to PATH COUNT times?'

EXAMPLE
	File 'JS'. After ./JcopyS JS . 3
	The 'ls' result will be:
	JS JS1 JS2 JS3

JcopyS

Created by JustSpace on 12.03.2019.
Copyright © 2019 Space. All rights reserved.
