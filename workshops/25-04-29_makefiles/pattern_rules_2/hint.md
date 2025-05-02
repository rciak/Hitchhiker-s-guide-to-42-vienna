# Pattern rules 2

* Continue story: Pirate cat being pissed by the the content of work_4.wuff
  decides to exclude it from the planned collection but to include only
  the other works.

Some particular hints:

* Variables set with `=` can be defined afterwards... (contrast to `:=`)
  
* Go through all "words" contained in the variable SRC and apply a pattern 
  substituion to each of these words: If a word contains the pattern `%.wuff`
  where `%` stands for anything replace it by `$(PCC_OBJDIR)/%.miau`, 
  where `%` stands for the very same anything.
  The words that are generated in that way are then stored in the makefile
  variable `PCC_OBJS` (**P**irat **C**at **C**opied **OBJ**ect**S**)

  ```make
  PCC_OBJS = $(patsubst %.wuff, $(PCC_OBJDIR)/%.miau, $(SRC))
  ```
* Explain that `\` allows to write a long line in several lines: 
  When `\` is **directly followed** by a newline character it is deactivating
  its effect (beware that there is no space character inbetween!!).

SRC := \
	work_1.wuff \
	work_2.wuff \
	work_3.wuff 
