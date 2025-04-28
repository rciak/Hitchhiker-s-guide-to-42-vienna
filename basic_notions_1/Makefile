# Structure of a Makefile rule:     |     Struktur einer Makefile Regel (GERMAN)
#                                   | 
# target: prerequisites             |     Zielobjekt: Erfordernisse
#     recipe line 1                 |         Rezept Zeile 1
#     recipe line 2                 |         Rezept Zeile 2
#     ...                           |         ...

#
# Normal Rules : For creating/updating files
#

concatenated: file_a file_b file_c
	cat file_a file_b file_c > concatenated
	echo "Created/updated file concatenated"

only_first_prerequisite: file_a file_b file_c
	cat file_a > only_first_prerequisite
	@echo "Created/updated file only_first_prerequisite"

