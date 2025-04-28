# Basic notions 2

1. **Remark:** Makefile has some variables that are automatically set before
  a recipe is executed. Here we see three very useful ones: The variable ...
  * ^ contains *all prerequisites* of the current rule
  * < contains just the *first prerequisite* of the current rule

2. Run

  ```zsh
  make concatenated
  ```

  ```zsh
  make only_first_prerequisite
  ```

3. Run rules again: Nothing to be done
  --> Same behaviour as before

4. Subst: 
   * concatenated --> $(@)
   * only_first_preresquisite --> $(@)

**Benefit of using this Autovariables:**
Compacter readable & more ease to adopt:
A file 4 can just be added to the list of prerequisites.
