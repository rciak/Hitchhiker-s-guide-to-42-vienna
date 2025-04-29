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

$(COLLECTION_NAME): $(PCC_OBJS)
	@echo "PCC_OBJS contains the prerequisites:"
	@echo $(PCC_OBJS)
	@echo "All prerequisites match our pattern rule and are built by it before"
	@echo "this recipe (rule all) is executed."
	tar -cf $(COLLECTION_NAME) $(PCC_OBJS)

pcc_obj/%.miau: %.wuff
#	@echo Creating folder $(PCC_OBJDIR) if it does not exist yet
	@mkdir -p $(PCC_OBJDIR)
	@echo Pirate copying:
	@echo "   $(<) --> $(@)"
	@cp $(<) $(@)    
