#
# Normal Rules : For creating/updating files
#
#
# Introducing PHONY Rules ...
#

COLLECTION_NAME := lib_of_all_pirated_copies.pcc

PCC_OBJDIR := pcc_obj
PCC_OBJS = $(patsubst %.wuff, $(PCC_OBJDIR)/%.miau, $(SRC))

SRC := \
	work_1.wuff \
	work_2.wuff \
	work_3.wuff 

.PHONY: all
all: $(COLLECTION_NAME)

$(COLLECTION_NAME): $(PCC_OBJS)
	@echo "PCC_OBJS contains the prerequisites:"
	@echo $(PCC_OBJS)
	@echo "All prerequisites match our pattern rule and are built by it before \
	this recipe (rule all) is executed."
	tar -cf $(COLLECTION_NAME) $(PCC_OBJS)

pcc_obj/%.miau: %.wuff
	@mkdir -p $(PCC_OBJDIR)
	@echo Pirate copying:
	@echo "   $(<) --> $(@)"
	@cp $(<) $(@)    

# Live add PHONY rules:
# clear_pirated_copies
# clear_pirated_copies_and_collection
# (for how it could look like scroll down...)































# .PHONY: clear_pirated_copies
# clear_pirated_copies:
# 	@echo "Deleting all pirated copies"
# 	@rm -f $(PCC_OBJS)

# # Version 1: Works but can be improved, see version 2
# .PHONY: clear_pirated_copies_and_collection
# clear_pirated_copies_and_collection:
# 	@echo "Deleting all pirated copies and the collection"
# 	@rm -f $(PCC_OBJS)
# 	@rm -f $(COLLECTION_NAME)

# # Version 2: The line @rm -f $(PCC_OBJS) is now only once in the Makefile
# .PHONY: clear_pirated_copies_and_collection
# clear_pirated_copies_and_collection: clear_pirated_copies
# 	@echo "Deleting the collection."
# 	@rm -f $(COLLECTION_NAME)













































