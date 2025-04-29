# Phony rules 1

* Continue story:  
  * For convenience, the rule all is added ; it seems to work...
  * `make all` 2 times..
  * ... but something is overlooked...
  * Dog Mulder from the FDI (Federal Dog-Department of Investigation) noticed
    that flaw in the rule all allowing im to stop its functioning...

* add file named `all` --> make all not working any more

* Pirate cat strikes back and makes `all` a phony target `.PHONY`, telling
  make to not regard it as a file:

  ```make
.PHONY: all
all: $(PCC_OBJS)
  ```