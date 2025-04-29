#
# Normal Rules : For creating/updating files
#
#
# Pattern Rules ...
#

PCC_OBJ_DIR := pcc_obj
# PCC_OBJS = $(patsubst %.wuff, $(PCC_OBJ_DIR)/%.miau, $(SRC))

# SRC := \
# 	work_1.wuff \
# 	work_2.wuff \
# 	work_3.wuff 

# all: $(PCC_OBJS)
# 	@echo "PCC_OBJS contains the prerequisites:"
# 	@echo $(PCC_OBJS)
# 	@echo "All prerequisites match our pattern rule and are built by it."

pcc_obj/%.miau: %.wuff
#	@echo Creating folder $(PCC_OBJ_DIR) if it does not exist yet
	@mkdir -p $(PCC_OBJ_DIR)
	@echo Pirate copying:
	@echo "   $(<) --> $(@)"
	@cp $(<) $(@)    
