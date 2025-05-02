* Run

  ```zsh
  make concatenated
  ```

  ```zsh
  make only_first_prerequisite
  ```

* Run rules again: Nothing to be done

* Change file_a and run again

**Remark:** A rule that *creates/updates a file* ideally is run again iff(*)  at least one of the prerequisites
has changed, since the last execution. Makefile's approach is comming close to this ideal: **It  compares the timestamp of the target with the timestamps of the prerequisites.**
--> If the timestamp of the target is newer than all the other timestamps it
assumes that nothing needs to be done.

**Technical note to (\*):**
This is not a typo: "iff" is short for "if and only if".
