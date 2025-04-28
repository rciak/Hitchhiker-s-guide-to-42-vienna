# Structure of a Makefile rule:     |     Struktur einer Makefile Regel (GERMAN)
#                                   | 
# target: prerequisites             |     Zielobjekt: Erfordernisse
#     recipe line 1                 |         Rezept Zeile 1
#     recipe line 2                 |         Rezept Zeile 2
#     ...                           |         ...

#
# Normal Rules : For creating/updating files
#

DEMO_VAR=Created/updated file concatenated.

concatenated: file_a file_b file_c
	cat $(^) > concatenated
	@echo $(DEMO_VAR)

only_first_prerequisite: file_a file_b file_c
	cat $(<) > only_first_prerequisite
	@echo $(LONG_TEXT)

DEMO_VAR2=Created/updated file only_first_prerequisite.
LONG_TEXT=$(DEMO_VAR2) 'Created/updated file only_first_prerequisite.\
 With some of course super important infos that would result in an annoyingly\
 long line \
1. - luckily make \
allows us to deactivate the newline character by putting the backslash symbol\
 directly in front of it. Be careful that you do not add an \
 invisible space between \ and the newline character! \
2. DEFINING VARIABLES SHOULD NORMALLY BE DONE BEFORE THE RULES. ;-) \
3. Be sure to set the text in quotes to avoid issues with special characters \
   like )'

