# Patttern rules 1

* Tell story, bringing the hiden rules up one by one by deleting inbetween \n 's

* Replace the three individual rules (uncomment) by the pattern rule

  ```make
pcc_obj/%.miau: %.wuff
	@echo Creating folder $(PCC_OBJ_DIR) if it does not exist yet
	@mkdir -p $(PCC_OBJ_DIR)
	@echo Pirate copying $(<) to $(@)
	cp $(<) $(@)
  ```

* **Remark:** Better use rsync instead of cp (cp is more for interactive use)