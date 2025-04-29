#
# Normal Rules : For creating/updating files
#
#
# Pattern Rules ...
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
	@echo "All prerequisites match our pattern rule and are built by it before"
	@echo "this recipe (rule all) is executed."
	tar -cf $(COLLECTION_NAME) $(PCC_OBJS)

pcc_obj/%.miau: %.wuff
	@mkdir -p $(PCC_OBJDIR)
	@echo Pirate copying:
	@echo "   $(<) --> $(@)"
	@cp $(<) $(@)    

# Live add PHONY rules:
# clear_pirated_copies
# clear_pirated_copies_and_collection