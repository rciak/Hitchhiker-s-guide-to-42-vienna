* Run

  ```zsh
  make concatenated
  ```

  ```zsh
  make only_first_prerequisite
  ```

* Run rules again: Nothing to be done

* Change file_a and run again

**Remark:** A rule needs to be run again if at least one of the prerequisites
has changed, since the last execution. Makefile is checking this by
comparing the timestamp of the target with the timestamp of the prerequisites:
If the timestamp of the target is newer than all the other timestamps it 
assumes that nothing needs to be done.

