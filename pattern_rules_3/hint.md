# Patttern rules 3

* Continue story:  
  Dog Mulder from the FDI (Federal Dog-Department of Investigation) noticed
  a flaw in the rule all allowing im to stop functioning...

* add file named `all` --> make all not working any more

* Pirate cat strikes back and makes `all` a phony target `.PHONY`, telling
  make to not regard it as a file:

  ```make
.PHONY: all
all: $(PCC_OBJS)
 	@echo "PCC_OBJS contains the prerequisites:"
 	@echo $(PCC_OBJS)
 	@echo "All prerequisites match our pattern rule and are built by it."
  ```